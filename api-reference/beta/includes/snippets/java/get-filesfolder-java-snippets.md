---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8aed909d0d46a2f7d9c93393e1223d7993a52ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976577"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.teams("{id}").channels("{id}").filesFolder()
    .buildRequest()
    .get();

```