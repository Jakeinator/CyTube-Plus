({
    init: function(){
        $('#nav-collapsible').append('<div class="navbar-text pull-right" id="utcClock"></div>');
        this.clock = $('#utcClock');
        this.tick();
    },
    tick: function(){
        this.now = new Date;
        this.clock.html(String().concat( this.now.getHours(), ":",
            this.now.getMinutes() > 9 ? this.now.getMinutes() : "0" + this.now.getMinutes(), ":",
            this.now.getSeconds() > 9 ? this.now.getSeconds() : "0" + this.now.getSeconds(), " :3"
            ));
        setTimeout(this.tick.bind(this), 1000);
    }

}).init();
