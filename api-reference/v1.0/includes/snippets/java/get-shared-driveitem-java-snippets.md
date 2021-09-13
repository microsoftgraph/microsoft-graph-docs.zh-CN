---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d689382536229b729747973533b86a40369190597b75d70607b62c1e7b4b5e6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163472"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.shares("{shareIdOrUrl}").driveItem()
    .buildRequest()
    .get();

```