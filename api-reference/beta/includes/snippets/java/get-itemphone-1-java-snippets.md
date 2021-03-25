---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a012a5033c629b9a1900c1bf84323d11da276eb
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209912"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPhone itemPhone = graphClient.me().profile().phones("{id}")
    .buildRequest()
    .get();

```