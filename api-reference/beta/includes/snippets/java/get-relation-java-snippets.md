---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b9fb446a063312fe9226bc6bbca6258fdf3f359
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981815"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RelationCollectionPage relations = graphClient.termStore().sets("{setId}").relations()
    .buildRequest()
    .get();

```