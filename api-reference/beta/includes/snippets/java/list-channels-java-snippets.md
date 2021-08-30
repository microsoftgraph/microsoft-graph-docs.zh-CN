---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6acbd2a4d274a999628141eccf90210574613df92b24bc73c5869e6802af3188
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219279"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelCollectionPage channels = graphClient.teams("893075dd-2487-4122-925f-022c42e20265").channels()
    .buildRequest()
    .get();

```