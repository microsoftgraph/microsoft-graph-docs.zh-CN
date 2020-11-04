---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cd98d993744439193890b9f0d05e7fa7659b8c4
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905906"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatMessageCollectionPage messages = graphClient.teams("303d2c1c-f1c5-40ce-b68e-544343d7f42b").channels("19:fec4b0f2825d4c8c82abc09027a64184@thread.skype").messages()
    .buildRequest()
    .get();

```