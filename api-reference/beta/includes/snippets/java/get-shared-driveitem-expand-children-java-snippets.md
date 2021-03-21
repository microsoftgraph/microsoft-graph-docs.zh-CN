---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69ff7342e4be08327993c4aa5a7d14d18cce611d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969482"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.shares("{shareIdOrUrl}").driveItem()
    .buildRequest()
    .expand("children")
    .get();

```