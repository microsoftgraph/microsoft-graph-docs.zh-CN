---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86d3be85c2a8b88152dd5432ceaf0b636410084c
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209946"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageDeltaCollectionPage delta = graphClient.teams("{id}").channels("{id}").messages()
    .delta()
    .buildRequest()
    .top(2)
    .get();

```