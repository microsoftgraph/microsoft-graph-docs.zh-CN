---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a22ccb4c3d995a10c5cfa8e663ea468f754d4aae
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983075"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String string = graphClient.compliance().ediscovery().cases("99e865fc-e29f-479a-ba83-9e58eb017103").operations("63926d4779c243458902328d83f61f53").microsoft.graph.ediscovery.caseExportOperation()
    .getDownloadUrl()
    .buildRequest()
    .get();

```