---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb348e25c2fc626df3f8a67f5ed380ba791c12b77cd604d165df42ce605792f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162404"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SourceCollection sourceCollection = new SourceCollection();
sourceCollection.displayName = "Quarterly Financials search";

graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("1a9b4145d8f84e39bc45a7f68c5c5119")
    .buildRequest()
    .patch(sourceCollection);

```