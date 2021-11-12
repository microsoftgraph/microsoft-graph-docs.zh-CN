---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb4293d53984e46bcefe79341e9dde7915870f5762e1fb9aec0ea1dd0f451da2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278087"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemEmail itemEmail = new ItemEmail();
itemEmail.displayName = "Business Email";
itemEmail.type = EmailType.WORK;

graphClient.users("{userId}").profile().emails("{id}")
    .buildRequest()
    .patch(itemEmail);

```