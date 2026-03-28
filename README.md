# gig_ocr_pack

Repositorio dedicado ao pack OCR portatil usado pelo `gig_app`.

## Objetivo

Manter o artefato OCR fora do repositorio principal do app, para que:

- o `gig_app` continue enxuto;
- o pack possa ser copiado, versionado e distribuido separadamente;
- o uso no computador do trabalho continue baseado em `GIG_OCR_PACK_ROOT`.

## Artefato atual

Pack validado localmente em `2026-03-26`:

- `gig_ocr_pack_app_dev_clean/`

Conveniencia local nao recomendada para versionamento em GitHub:

- `gig_ocr_pack_app_dev_clean.zip`

## Origem do build

O pack foi gerado a partir de:

- `C:\Workspace\repos\gig_app`

Arquivos-fonte principais no app:

- `scripts/build_ocr_pack.py`
- `pdf_text_converter.py`
- `docs/operacional/OCR_PORTATIL_TRABALHO.md`

## Uso com gig_app

1. Validar o pack com `gig_ocr_pack_app_dev_clean\check_ocr_pack.bat`.
2. Rodar `gig_ocr_pack_app_dev_clean\run_gig_with_ocr_pack.bat <CAMINHO_DO_REPO_DO_APP>`.

Alternativa:

1. Rodar `gig_ocr_pack_app_dev_clean\activate_ocr_pack.bat`.
2. Abrir o `gig_app` no mesmo terminal.

## Regra pratica

- a pasta descompactada e o artefato principal do repo;
- o `.zip` fica apenas como conveniencia local;
- se este repositorio for para GitHub comum, evitar versionar o `.zip`, porque ele excede o limite confortavel para repositorio binario leve.
