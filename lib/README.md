#  Libraries

## Maybe

- maybe :: forall a b. b -> (a -> b) -> Maybe a -> b
- fromMaybe :: forall a. a -> Maybe a -> a
- isJust :: forall a. Maybe a -> Boolean
- isNothing :: forall a. Maybe a -> Boolean

## Array

- singleton :: forall a. a -> Array a
- range :: Int -> Int -> Array Int
- replicate :: forall a. Int -> a -> Array a
- null :: forall a. Array a -> Boolean
- length :: forall a. Array a -> Int
- cons :: forall a. a -> Array a -> Array a
- snoc :: forall a. Array a -> a -> Array a
- head :: forall a. Array a -> Maybe a
- last :: forall a. Array a -> Maybe a
- tail :: forall a. Array a -> Maybe (Array a)
- init :: forall a. Array a -> Maybe (Array a)
- index :: forall a. Array a -> Int -> Maybe a
- insertAt :: forall a. Int -> a -> Array a -> Maybe (Array a)
- deleteAt :: forall a. Int -> Array a -> Maybe (Array a)
- updateAt :: forall a. Int -> a -> Array a -> Maybe (Array a)
- reverse :: forall a. Array a -> Array a
- filter :: forall a. (a -> Boolean) -> Array a -> Array a
- sort :: forall a. Ord a => Array a -> Array a
- take :: forall a. Int -> Array a -> Array a
- map :: forall a b.(a -> b) -> Array a -> Array b

## Tuple

- fst :: forall a b. Tuple a b -> a
- snd :: forall a b. Tuple a b -> b
- swap :: forall a b. Tuple a b -> Tuple b a

## List

- nil :: forall a. List a
- cons :: forall a. a -> List a -> List a
- map :: forall a b . (a -> b) -> List a -> List b
- length :: List a -> Int
- foldl :: forall a b.(b -> a-> b) -> b -> List a -> b
- foldr :: forall a b.(a -> b -> b) -> b -> List a -> b
- scanl :: forall a b.(b -> a -> b) -> b -> List a -> List b
- scanr :: forall a b.(a -> b -> b) -> b -> List a -> List b
- head ::forall a.List a -> Maybe a
- last :: forall a.List a -> Maybe a
- reverse :: forall a.List a -> List a
- concat :: forall a.List (List a) -> List a
- filter :: forall a. (a -> Boolean) -> List a -> List a
- connect ::forall a.List a -> List a -> List a
- and :: List Boolean -> Boolean
- or :: List Boolean -> Boolean
- any :: forall a.(a -> Boolean) -> List a -> Boolean
- all :: forall a.(a -> Boolean) -> List a -> Boolean
- replicate :: forall a. Int -> a -> List a
- take :: forall a. Int -> List a -> List a
- drop :: forall a. Int -> List a -> List a

## Binary

- band :: Bits -> Bits -> Bits
- bor :: Bits -> Bits -> Bits
- bnot :: Bits -> Bits
- bxor :: Bits -> Bits -> Bits
- bsl :: Bits -> Int -> Bits
- bsr :: Bits -> Int -> Bits

## Map

- empty :: forall k v. Map k v
- isEmpty :: forall k v. Map k v -> Boolean
- insert :: forall k v.k -> v -> Map k v -> Map k v
- lookup :: forall k v. k -> Map k v -> Maybe v
- delete :: forall k v.k -> Map k v -> Map k v
- update :: forall k v. (v -> Maybe v) -> k -> Map k v -> Map k v
- size :: forall k v. Map k v -> Int
- filter :: forall k v.(v -> Boolean) -> Map k v -> Map k v

## String

- connect :: String -> String -> String
- take :: Int -> String -> Maybe String
- reverse :: String -> String
- append :: String -> String -> String
- length :: Stirng -> Int

