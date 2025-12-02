## TICKET
- URL: 

## 📦 COMMON *(Mục 3, 4, 11, 17.1, 19, 23)*
- [ ] File mới đặt đúng package theo cấu trúc: `{domain}/{model|persistence|func|util}` (mục 11)
- [ ] Đặt tên Model, Repository, Table, DTO, Enum tuân thủ conventions (mục 4)
- [ ] Code thẳng hàng dọc (`=`, `=>`, `->`), sử dụng 2 spaces cho indentation (mục 23)
- [ ] Sử dụng Scala 3 Features: Opaque Types, Enum, Given/Using, Extension Methods, Phantom Types (mục 3)
- [ ] Thứ tự import: Standard → Third-party → Framework (ixias) → Internal domain → Internal utils (mục 17.1)
- [ ] Ghi log với `ixias.core.util.Log.*` và `RequestLogger` (mục 19)

## 📚 ĐỐI VỚI LIB

- [ ] Companion object định nghĩa: `type Id`, `type WithNoId`, `type EmbeddedId` (mục 2.2)
- [ ] Enum đặt ở Object level, không lồng trong SearchCriteria (mục 2.3)
- [ ] SearchCriteria extends `JsonDecoder`, định nghĩa `given Decoder`, `given PaginationConfig` (mục 8)
- [ ] Repository: `open case class`, extends `SlickRepository`, có methods đầy đủ (mục 2.1, 17.2)
- [ ] Search dùng `filterOpt` cho optional criteria (mục 9.2)
- [ ] Soft delete pattern: `softDelete()`, `restore()`, filter `deletedAt.isEmpty` (mục 9.3)
- [ ] Read dùng `HOSTSPEC_REPLICA`, Write dùng `HOSTSPEC_PRIMARY` (default) (mục 9.1)
- [ ] Table có Search Extension Trait riêng, sử dụng `TableProvider` (mục 10.2, 10.3)
- [ ] Model > 22 fields dùng `splitAt`, `concat`, `Mirror.ProductOf` (mục 18)
- [ ] Repository Container pattern với `@Singleton` (mục 2.4)

## DOCUMENT CODE PATTERN
https://github.com/hybrid-tech-rezil/rezil-docs/pull/44/
