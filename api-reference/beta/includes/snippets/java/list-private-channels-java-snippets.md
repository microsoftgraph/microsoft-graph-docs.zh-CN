---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1f86186d146949fc953ae8f19816208d94a9d0c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967290"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelCollectionPage channels = graphClient.teams("{id}").channels()
    .buildRequest()
    .filter("membershipType eq 'private'")
    .get();

```