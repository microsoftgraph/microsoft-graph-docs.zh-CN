---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e334155d83b78643b41cd85580fc9842175219ee
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211897"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelCollectionPage channels = graphClient.teams("6a720ba5-7373-463b-bc9f-4cd04b5c6742").channels()
    .buildRequest()
    .filter("membershipType eq 'shared'")
    .get();

```