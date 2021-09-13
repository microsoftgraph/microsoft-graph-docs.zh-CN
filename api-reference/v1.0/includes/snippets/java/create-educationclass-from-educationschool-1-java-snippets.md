---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af94a2a2758864dcc22e735712c991568efdbce0a4fa5b97d48fbf7fbfe87de5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332440"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{class-id}").members("{member-id}")
    .buildRequest()
    .delete();

```