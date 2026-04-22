> Saving the world one commit at a time (with questionable commit messages).

```ocaml
(* ~/bio/whoami.ml *)

type engineer = {
  role: string;
  location: string;
}

let me = {
  role = "Software Engineer";
  location = "Nairobi, Kenya";
  stack = ["Ruby"; "Scala"; "Go", "Clojure"; "Python"];
}

let () =
  Printf.printf "Hey, there 👋 I'm a %s based in %s.\n" me.role me.location;
  Printf.printf "Currently hacking in: %s\n" (String.concat ", " me.stack);
```

![Clov's Github activity graph](https://github-readme-activity-graph.vercel.app/graph?username=clovisphere&theme=github-compact)
