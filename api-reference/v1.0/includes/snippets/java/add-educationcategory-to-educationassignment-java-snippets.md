---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cd8bd4f14db6f794491031bd262bb4d0b8b7572996840bf806f2d32d5fb097b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332084"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").categories("ec98f158-341d-4fea-9f8c-14a250d489ac").reference()
    .buildRequest()
    .delete();

```