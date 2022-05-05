---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70a5d728ee3c35a2f1c58ce37947507066aab59b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212607"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelCollectionWithReferencesPage allChannels = graphClient.teams("893075dd-2487-4122-925f-022c42e20265").allChannels()
    .buildRequest()
    .get();

```