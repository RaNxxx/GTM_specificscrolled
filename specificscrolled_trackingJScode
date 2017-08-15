<script>
    /**
     * author Remy Sharp
     * url http://remysharp.com/2009/01/26/element-in-view-event-plugin/
     * fork https://github.com/zuk/jquery.inview
     */
    (function(e) {
        function m() {
            var b = window.innerHeight;
            if (b) return b;
            var f = document.compatMode;
            if (f || !e.support.boxModel) b = "CSS1Compat" === f ? document.documentElement.clientHeight : document.body.clientHeight;
            return b
        }
        var n = function(b, f) {
            function e() {
                null !== a ? c = !0 : (c = !1, b(), a = setTimeout(function() {
                    a = null;
                    c && e()
                }, f))
            }
            var c = !1,
                a = null;
            return e
        }(function() {
            var b = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop,
                f = b + m(),
                g = [];
            e.each(e.cache, function() {
                this.events && this.events.inview &&
                    g.push(this.handle.elem)
            });
            e(g).each(function() {
                var c = e(this),
                    a;
                a = 0;
                for (var d = this; d; d = d.offsetParent) a += d.offsetTop;
                var d = c.height(),
                    k = a + d,
                    d = c.data("inview") || !1,
                    h = c.data("offset") || 0,
                    g = a > b && k < f,
                    l = k + h > b && a < b,
                    h = a - h < f && k > f;
                g || l || h || a < b && k > f ? (a = h ? "top" : l ? "bottom" : "both", d && d === a || (c.data("inview", a), c.trigger("inview", [!0, a]))) : !g && d && (c.data("inview", !1), c.trigger("inview", [!1]))
            })
        }, 100);
        e(window).on("checkInView.inview click.inview ready.inview scroll.inview resize.inview", n)
    })(jQuery);

    var sent = {},
        timer = {};

    // 計測したい箇所1
    var o1 = "#youneedtochangeit01";
    sent[o1] = false;
    jQuery(o1).bind('inview', function(event, visible) {
        var o = o1;
        if (visible) {
            clearTimeout(timer[o]);
            timer[o] = setTimeout(function() {
                if (!sent[o]) { // 計測したい箇所1
                    dataLayer.push({
                        'event': 'scrolled_specific',
                        'event_specificarea': '計測したい箇所1',
                        'object': o
                    });
                    sent[o] = true;
                }
            }, 3000);
        } else {
            clearTimeout(timer[o]);
        }
    });

    // 計測したい箇所2
    var o2 = "#youneedtochangeit02";
    sent[o2] = false;
    jQuery(o2).bind('inview', function(event, visible) {
        var o = o2;
        if (visible) {
            clearTimeout(timer[o]);
            timer[o] = setTimeout(function() {
                if (!sent[o]) { // 計測したい箇所2
                    dataLayer.push({
                        'event': 'scrolled_specific',
                        'event_specificarea': '計測したい箇所2',
                        'object': o
                    });
                    sent[o] = true;
                }
            }, 3000);
        } else {
            clearTimeout(timer[o]);
        }
    });

    // 計測したい箇所3
    var o3 = "#youneedtochangeit03";
    sent[o3] = false;
    jQuery(o3).bind('inview', function(event, visible) {
        var o = o3;
        if (visible) {
            clearTimeout(timer[o]);
            timer[o] = setTimeout(function() {
                if (!sent[o]) { // 計測したい箇所3
                    dataLayer.push({
                        'event': 'scrolled_specific',
                        'event_specificarea': '計測したい箇所3',
                        'object': o
                    });
                    sent[o] = true;
                }
            }, 3000);
        } else {
            clearTimeout(timer[o]);
        }
    });
</script>
