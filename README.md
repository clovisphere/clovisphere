~/whoami

> A small Zig file pretending to be a README,  
> and a README pretending to be a résumé.

Written by someone who believes good software is mostly deleting code,
naming things carefully, and letting tests do the arguing.

```zig

const std = @import("std");

pub const Clov = struct {
    /// Identity
    role: []const u8 = "Software Engineer",
    focus: []const u8 = "backend systems built to be tested, trusted, and boring in production.",

    /// Narrative truth
    mission: []const u8 = "Saving the world one commit at a time (with questionable commit messages).",

    /// Core stack
    languages: []const []const u8 = &.{
        "Ruby",
        "Haskell",
        "Go",
        "Zig",
    },

    paradigms: []const []const u8 = &.{
        "Object-Oriented",
        "Functional",
        "Logical",
    },

    /// Performance specs (benchmarked in production, not vibes)
    reliability: u8 = 100, // cosmic-storm resistant
    test_coverage: f32 = 1.0, // lie-detector approved

    pub fn buildSystem(self: @This()) void {
        std.log.info(
            "Whispering to gophers, charming snakes, and arguing politely with compilers…",
            .{},
        );

        self.deployResilientAPI();
    }

    fn deployResilientAPI(_: @This()) void {
        std.log.info(
            "Shipping something boring, stable, and still standing at 3 a.m.",
            .{},
        );
    }
};
```

![Clov's Github activity graph](https://github-readme-activity-graph.vercel.app/graph?username=clovisphere&theme=github-compact)
