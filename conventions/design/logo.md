# Logo
<table>
	<thead>
		<tr>
			<th>Status</th>
			<th>Verification</th>
			<th>Authors</th>
			<th>Created date</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td><i>Published</i></td>
			<td><i>Until Nov 17, 2025</i></td>
			<td><i><a href="https://www.github.com/Xibitol">Xibitol</a></i></td>
			<td><i>Feb 25, 2024</i></td>
		<tr>
	</tbody>
</table>

## Convention
There aren’t really any common conventions on logos, banners or anything related
to branding. Thus, we chosen to follow Android’s icon design
specifications<sup>1</sup> that seems to fit greatly to our designs and our
branding styles, and we extended it to cover every aspects of our brand.

_Everything is summed up in a table at [Summary](#summary) and at
[Specific sizes](#specific-sizes) for specific sizes._

### Files
In a general manner, every brand files must have a `SVG` version. It’s really
useful as it allows us to include it every where we want, without thinking about
having the good size.

Exported from them, brand files may also have a `PNG` version in a `sRGB` colour
space when apps or services doesn’t accept vector images. In these cases, images
have file size limits.

Moreover, each files must have a **clear and unique name**, even between
projects. The file name format is
```
<project>[_<type>]_logo[_<width>-<height>].<ext>
```
where:

- `project` is the associated project name like `Pimous`.
- `type` is the type of the logo if it’s not the base one.
- `width` and `height` are the dimensions of the logo if these are not
referenced in the Pimous conventions, like in theses cases:
[Specific sizes](#specific-sizes). When there are referenced but there aren’t
the base one, the `type` option is preferred.
- `ext` is one of the supported file extension based on the type and the system.

_([PCRE](http://www.pcre.org/) regular expression : `^(?'project'[a-zA-Z0-9-]+)(?>_(?'type'[a-zA-Z]+))?_logo(?>_(?'width'[1-9][0-9]*)-(?'height'[1-9][0-9]*))?\.(?'ext'[a-z]{3,})$`)_

### Dimensions

Android’s icon design specifications<sup>1</sup> say that an icon, or a logo in
our case, must be sized to a square of **512 pixels** and its centred content
has to fit in **75% of the main size**, a ratio of `0.75`; so the content must
be centred and sized to a square of **384 pixels ($512\times0.75$)**.

On that baseline, we extend it to a larger logo as a banner. It must be sized to
a rectangle of **1536 per 512 pixels ($512\times3$)**, and its content, also
centred, must be sized to a rectangle of **1408 per 384 pixels
($512\times(3-0.25)$ per $512\times0.75$)**.

Furthermore, we add a background image as a “Full-screen logo” that don’t follow
the baseline. So it must be sized to a rectangle of **1920 per 1080 pixels
(16/9)**.

#### Specific sizes
In addition, some systems need specific sizes of logos that are referenced
below:
| **System** | **Dimensions** | **Large dimensions** |
| --- | --- | --- |
| Garry’s Mod<sup>2</sup>  | square of 24 (or 32) | 128 per 288 to 1024 |

### Summary
| **Type** | **Format** | **File size** | **Dimensions** | **Content dimensions** | **Description** |
| --- | --- | --- | --- | --- | --- |
| Base (No `type`) | `SVG` or `PNG` | 1024 KB | 512/512 | 384/384 | Base logo without the project name. |
| Transparent | `SVG` or `PNG` | 1024 KB | 512/512 | 384/384 | Base logo with a transparent background, used for an incrustation. |
| Small | `SVG` or `PNG` | 1024 KB | 512/512 | 384/384 | Base logo reduced to include the project name; Usually the logo at the top and the title at the bottom. |
| Large (Banner) | `SVG` or `PNG` | 3072 KB | 1536/512 | 1408/384 | Base logo associated with the project name; Usually the logo at the left and the title at the right. |
| Full-screen (Background) | `SVG` or `PNG` | Not limited | 1920/1080 | 1920/1080 | An image representing the project with its name and its base logo somewhere; Usually centred. |

## References
1. “Google Play icon design specifications”, Android Developers. [Online]. Available: https://developer.android.com/distribute/google-play/resources/icon-design-specifications. [Accessed: 17-Nov-2024];
2. “Gamemode creation”, Garry’s Mod Wiki. [Online]. Available: https://wiki.facepunch.com/gmod/Gamemode_Creation. [Accessed: 17-Nov-2024].