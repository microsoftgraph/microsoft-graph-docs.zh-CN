---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f764c5abd412a442004f691b44e0cb683da93d3e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212569"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelCollectionWithReferencesPage allChannels = graphClient.teams("893075dd-2487-4122-925f-022c42e20265").allChannels()
    .buildRequest()
    .filter("membershipType eq 'shared'")
    .get();

```