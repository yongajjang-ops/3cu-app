# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

3쿠션 당구 연습 노트 (3-Cushion Billiards Practice Note) - A web application for recording and managing billiard ball positions and practice notes.

## Running the App

Open `index.html` directly in a browser. No server or build step needed.

## Tech Stack

- Vanilla JavaScript (no framework)
- Tailwind CSS (via CDN)
- HTML5 Canvas for billiard table rendering
- localStorage for data persistence

## Features

1. **Ball Placement**: Place red, yellow, and white balls on the table
2. **Drag & Drop**: Drag balls to reposition them
3. **Delete Mode**: Remove individual balls
4. **Memo Input**: Name, notes, and difficulty level for each layout
5. **Save/Load**: Save layouts to localStorage and reload them
6. **Responsive Design**: Works on both desktop and mobile devices

## Architecture

### Single File Structure
Everything is contained in `index.html`:
- HTML meta tags and CDN scripts
- CSS styles in `<style>` tag
- JavaScript in `<script>` tag

### Code Organization
1. **Constants**: Ball radius, table dimensions, colors
2. **State Variables**: Canvas, balls, drag state, selected mode
3. **Canvas Functions**: Table and ball rendering
4. **Event Handlers**: Click, drag, touch events
5. **Utility Functions**: Position checking, status updates
6. **Storage Functions**: Save, load, delete layouts

### Key Functions
- `initCanvas()`: Initialize canvas and event listeners
- `drawTable()`: Render the billiard table
- `drawBall()`: Render individual ball with gradient
- `handleCanvasClick()`: Handle ball placement and deletion
- `handleMouseDown/Move/Up()`: Handle drag operations
- `saveLayout()`: Save current layout to localStorage
- `loadLayout()`: Restore layout from saved data
