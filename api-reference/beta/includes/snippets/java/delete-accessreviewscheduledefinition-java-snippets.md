---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b85048394e8fc671df1033c891d66a42fe9e1f170bee78e09e202a7b518ee22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104119"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("29f2d16e-9ca6-4052-bbfe-802c48981fd8")
    .buildRequest()
    .delete();

```