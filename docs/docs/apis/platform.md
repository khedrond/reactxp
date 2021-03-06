---
id: apis/platform
title: Platform
layout: docs
category: Interfaces
permalink: docs/apis/platform.html
next: apis/popup
---

This interface provides information about the OS or runtime platform on which the app is running.

## Types
``` javascript
type PlatformType = 'web' | 'ios' | 'android' | 'windows';
```

## Methods
``` javascript
// Returns the platform type
getType(): Types.PlatformType;

// Returns the value in `specifics` for the current platform type.
select<T>(specifics: { [ platform in Types.PlatformType | 'default' ]?: T }): T | undefined;
```

