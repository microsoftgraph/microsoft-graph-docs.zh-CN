---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b67274588b5f050de661f3e5d5b3ca938e5125529e6313c56287e819467b934
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219280"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelCollectionPage channels = graphClient.teams("64c323f2-226a-4e64-8ba4-3e6e3f7b9330").channels()
    .buildRequest()
    .filter("membershipType eq 'private'")
    .get();

```