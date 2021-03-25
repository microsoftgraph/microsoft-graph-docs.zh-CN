---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de53747c567323375ba03950bee8175b88e2b9e3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209307"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceEndpointCollectionPage endpoints = graphClient.print().services("{id}").endpoints()
    .buildRequest()
    .get();

```