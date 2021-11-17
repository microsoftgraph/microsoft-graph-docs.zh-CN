---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38dc01f4e38467d2a80c127f65708a76642b7eee0819a1119eae7deb89a559d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902736"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2975E9B5-44CE-4E71-93D3-30F03B5AA992")
    .buildRequest()
    .delete();

```