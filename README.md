# React Router Dom: Unexpected Route Behavior

This repository demonstrates a common issue encountered when using React Router Dom v6 and above: unexpected behavior when navigating to a route that hasn't been explicitly defined.

## Problem

The provided `App.js` includes routes for '/' and '/about', but lacks a route for '/contact'.  Attempts to navigate to '/contact' can lead to different problematic behaviors depending on the surrounding application setup. It might display a blank screen, show a previous page, or throw an error.

## Solution

The ideal solution is to add a route for `/contact`.  If you want to handle undefined routes, you can add a catch-all route using `*` as a path which acts as a 404 page.