CREATE Sequence produtoId
start with 1
increment by 1;

CREATE Sequence vendaId
start with 1
increment by 1;

CREATE TABLE Produto (
	Id number primary key,
	Nome Varchar2(120),
	Tipo Varchar2(120),
	Quantidade number,
	DataGeracao date
);

CREATE TABLE Venda (
	Id number primary key,
	DataVenda date,
	IdProduto number,
	FOREIGN KEY (IdProduto) REFERENCES Produto(Id)
);

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Camiseta', 'Vestuário', 20, TO_DATE('2022-01-01', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Celular', 'Eletrônicos', 15, TO_DATE('2022-01-02', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Notebook', 'Eletrônicos', 10, TO_DATE('2022-01-03', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Tênis', 'Calçados', 30, TO_DATE('2022-01-04', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Mesa', 'Móveis', 25, TO_DATE('2022-01-05', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'TV', 'Eletrônicos', 12, TO_DATE('2022-01-06', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Óculos de Sol', 'Acessórios', 40, TO_DATE('2022-01-07', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Bola de Futebol', 'Esportes', 20, TO_DATE('2022-01-08', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Relógio', 'Acessórios', 18, TO_DATE('2022-01-09', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Cadeira', 'Móveis', 35, TO_DATE('2022-01-10', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Fones de Ouvido', 'Acessórios', 25, TO_DATE('2022-01-11', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Mouse', 'Eletrônicos', 30, TO_DATE('2022-01-12', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Livro', 'Cultura', 50, TO_DATE('2022-01-13', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Chapéu', 'Acessórios', 15, TO_DATE('2022-01-14', 'YYYY-MM-DD'));

INSERT INTO Produto (Id, Nome, Tipo, Quantidade, DataGeracao) VALUES
(produtoId.NEXTVAL, 'Câmera Fotográfica', 'Eletrônicos', 8, TO_DATE('2022-01-15', 'YYYY-MM-DD'));

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-01', 'YYYY-MM-DD'), 1);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-02', 'YYYY-MM-DD'), 2);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-03', 'YYYY-MM-DD'), 3);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-04', 'YYYY-MM-DD'), 4);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-05', 'YYYY-MM-DD'), 5);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-06', 'YYYY-MM-DD'), 6);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-07', 'YYYY-MM-DD'), 7);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-08', 'YYYY-MM-DD'), 8);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-09', 'YYYY-MM-DD'), 9);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-10', 'YYYY-MM-DD'), 10);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-11', 'YYYY-MM-DD'), 11);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-12', 'YYYY-MM-DD'), 12);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-13', 'YYYY-MM-DD'), 13);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-14', 'YYYY-MM-DD'), 14);

INSERT INTO Venda (Id, DataVenda, IdProduto) VALUES
(vendaId.NEXTVAL, TO_DATE('2022-01-15', 'YYYY-MM-DD'), 15);
