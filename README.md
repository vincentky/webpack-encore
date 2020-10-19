# Webpack Encore: A Simple & Powerful Webpack API

[![Build Status](https://travis-ci.org/symfony/webpack-encore.svg?branch=master)](https://travis-ci.org/symfony/webpack-encore)
[![NPM Version](https://badge.fury.io/js/%40symfony%2Fwebpack-encore.svg)](https://badge.fury.io/js/%40symfony%2Fwebpack-encore)
![Node](https://img.shields.io/node/v/@symfony/webpack-encore.svg)

Add Imagemin option for webpack encore

## Example

```js
...

Encore.enableImagemin({
          mozjpeg: {
            progressive: true,
            quality: 65
          },
          optipng: {
            enabled: false
          },
          pngquant: {
            quality: [0.10, 0.20],
            speed: 4
          },
          gifsicle: {
            interlaced: false
          },
          svgo: {
            plugins:
              [
                {
                  removeViewBox: false
                }
              ]
          }
        })

Webpack Encore is a simpler way to integrate [Webpack](https://webpack.js.org/) into your
application. It *wraps* Webpack, giving you a clean & powerful API
for bundling JavaScript modules, pre-processing CSS & JS and compiling
and minifying assets. Encore gives you a professional asset system
that's a *delight* to use.

Encore is inspired by [Webpacker](https://github.com/rails/webpacker) and
[Mix](https://laravel.com/docs/mix), but stays in the spirit of
Webpack: using its features, concepts and naming conventions for a familiar
feel. It aims to solve the most common Webpack use cases.

> Encore is made by Symfony and works *beautifully* in Symfony applications.
> But it can easily be used in any application... in any language!

## Documentation

[Read the Documentation on symfony.com](https://symfony.com/doc/current/frontend.html)
or view a demo application: [symfony/demo](https://github.com/symfony/demo).
