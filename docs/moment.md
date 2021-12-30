# moment

Moment has various lighter replacements these days. The one I would highly
recommend is [date-fns](https://github.com/date-fns/date-fns).

date-fns supports ESM out of the box and ships its own TypeScript definitions.

The hope is that one day these can also depend on the new `Intl` and/or
temporal web APIs to further reduce their bundle sizes.

## Alternatives

- [date-fns](https://github.com/date-fns/date-fns)
- [dayjs](https://github.com/iamkun/dayjs)
- [luxon](https://github.com/moment/luxon)

## Native alternatives (future)

In future, we should be able to use the new
[temporal](https://tc39.es/proposal-temporal/docs/index.html) APIs to reduce
or completely replace the need for these libraries.
