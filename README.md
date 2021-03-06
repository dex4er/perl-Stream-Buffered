# NAME

Stream::Buffered - temporary buffer to save bytes

# SYNOPSIS

    my $buf = Stream::Buffered->new($length);
    $buf->print($bytes);

    my $size = $buf->size;
    my $fh   = $buf->rewind;

# DESCRIPTION

Stream::Buffered is a buffer class to store arbitrary length of byte
strings and then get a seekable filehandle once everything is
buffered. It uses PerlIO and/or temporary file to save the buffer
depending on the length of the size.

# SEE ALSO

[Plack::Request](https://metacpan.org/pod/Plack::Request)

# AUTHOR

Tatsuhiko Miyagawa

This module is part of [Plack](https://metacpan.org/pod/Plack), released as a separate distribution for easier
reuse.

# COPYRIGHT

The following copyright notice applies to all the files provided in
this distribution, including binary files, unless explicitly noted
otherwise.

Copyright 2009-2011 Tatsuhiko Miyagawa

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.
