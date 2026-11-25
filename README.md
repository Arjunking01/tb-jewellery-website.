# TB Jewellery Product Media Repository

This repository stores public product photographs
used by the TB Jewellery catalogue website.

## Website Integration

The website uses GitHub Contents API through its
server-side backend.

The owner admin panel supports:

- Product image uploads
- Image replacement
- Image retrieval
- Safe image deletion
- Product image URL synchronization

## Repository Configuration

Repository:
Arjunking01/tb-jewellery-website.

Default branch:
main

Storage directory:
products/

## Vercel Configuration

Required environment variables:

GITHUB_TOKEN
GITHUB_MEDIA_REPO
GITHUB_MEDIA_BRANCH

GITHUB_MEDIA_REPO=Arjunking01/tb-jewellery-website.
GITHUB_MEDIA_BRANCH=main

The GitHub token must remain server-side.

Never expose credentials in browser code.

## Image Management

The website must:

1. Validate uploaded photographs.
2. Upload images using unique filenames.
3. Verify successful uploads.
4. Save image URLs in the catalogue.
5. Check references before deleting images.
6. Verify successful deletion.

Never delete an image that is still referenced
by another catalogue product.
