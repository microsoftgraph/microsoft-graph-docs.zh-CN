---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f6b53cf55eeb0358770dc2e4c7de8794d8663b2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959290"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.teams("{id}").channels("{id}").filesFolder()
    .buildRequest()
    .get();

```