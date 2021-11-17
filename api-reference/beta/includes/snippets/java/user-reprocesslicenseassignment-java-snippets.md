---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6933ec852c3a98d931b04310b95d0c38bd18eb82b32cbd5fa8ba9c52a304f3e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161357"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("047dd774-f1c4-40f2-82f0-278de79f9b83")
    .reprocessLicenseAssignment()
    .buildRequest()
    .post();

```