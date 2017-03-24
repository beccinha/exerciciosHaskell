-- funcao para buscar um elemento de uma lista
elementAt :: [a] -> Int -> a
elementAt (h:t) x = if (x==1) then h 
                             else elementAt t (x-1)
 
 -- funcao para reverter uma lista
 myReverse :: [a] -> [a]
myReverse [] = []
myReverse [a] = [a]
myReverse (h:t) = myReverse t ++ [h]

-- funcao para o palindromo
isPalindromo :: Eq a=> [a] -> Bool
isPalindromo [] = True
isPalindromo [a] = True
isPalindromo (h:t) | myReverse (h:t) == (h:t) = True
                   | True = False
    
-- funcao para flatten a nested list structure
-- funcao para tirar os elementos repetidos juntos de uma lista
compress :: Eq a =>[a] -> [a]
compress [] = []
compress [a] = [a]
compress (h:t) | h == head t = compress t 
               | True = h :compress t 
 
--funcao para separar os elementos repidos seguidos
