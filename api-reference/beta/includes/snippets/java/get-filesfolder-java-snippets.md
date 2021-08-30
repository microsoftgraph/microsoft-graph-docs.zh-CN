---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1327fa3f1b2897ab7e54ad51879c3c12990424bbe9534235042bcb444767edc0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277482"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.teams("{id}").channels("{id}").filesFolder()
    .buildRequest()
    .get();

```