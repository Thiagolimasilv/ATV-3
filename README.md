# ATV-3
-- Adicionar coluna 'favorites' à tabela 'alunos'
ALTER TABLE alunos
ADD COLUMN favorites VARCHAR(255);

-- Atualizar os 10 amigos favoritos para cada aluno
UPDATE alunos
SET favorites = 'SIM'
WHERE nome IN ('Adrielly', 'Daiana', 'Enzo', 'Geovana Vieira', 'Hugo', 'Isabella Bertolo', 'Pedro Arthur', 'Ryan', 'Thiago', 'Wesley', 'Geovanna');

-- Mostrar os dados atualizados
SELECT * FROM alunos;
