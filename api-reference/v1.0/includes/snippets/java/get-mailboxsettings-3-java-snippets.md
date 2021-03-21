---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 074be432784b274948fae9ebc2f155acbbe86d56
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967649"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkingHours workingHours = graphClient.customRequest("/me/mailboxSettings/workingHours", WorkingHours.class)
    .buildRequest()
    .get();

```