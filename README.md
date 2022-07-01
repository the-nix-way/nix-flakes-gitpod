# Nix with flakes enabled on GitPod

This [GitPod] environment has [Nix] installed and [flakes] enabled.

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/the-nix-way/nix-flakes-gitpod)

The environment is quite simple and has just two packages available: `hello` and `cowsay`.

To run the environment in your browser, click on the GitPod button above. Once the environment is ready, open the terminal and you'll be automatically dropped into the flake-provided Nix shell.

Then you can see that the flake-provided packages are available. Run the `hello` package:

```shell
bash-5.1$ hello
Hello, world!
```

Run the `cowsay` package with an input:

```shell
bash-5.1$ cowsay mooooo
 ________
< mooooo >
 --------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

## Origins

This config is based on GitPod's [official Nix template][template]. It makes just [one small change][change] to the template to enable [flakes] and also provides a simple [`flake.nix`](./flake.nix) for use in the project.

## Template

Like GitPod's original, you can use this repo as a template by clicking on **Use this template** above.

[change]: https://github.com/the-nix-way/nix-flakes-gitpod/blob/main/.gitpod.yml#L8
[flakes]: https://nixos.wiki/wiki/Flakes
[gitpod]: https://gitpod.io
[nix]: https://nixos.org
[template]: https://github.com/gitpod-io/template-nix

