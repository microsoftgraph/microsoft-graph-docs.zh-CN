---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35fbe5b87c5aae35c0950bcfde278b73a4aa3ff6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979802"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChannelCollectionPage channels = graphClient.teams("{id}").channels()
    .buildRequest()
    .filter("membershipType eq 'private'")
    .get();

```