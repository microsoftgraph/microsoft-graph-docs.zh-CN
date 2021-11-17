---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad9541bbbdc326380308e24e33d390a2faca7b1a0329bad457d85245e8941655
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278010"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealth serviceHealth = graphClient.admin().serviceAnnouncement().healthOverviews("Microsoft 365 suite")
    .buildRequest()
    .get();

```