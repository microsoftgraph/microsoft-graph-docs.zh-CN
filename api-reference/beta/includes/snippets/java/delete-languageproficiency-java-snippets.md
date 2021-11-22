---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64c0bf678c3cc74f463cde66f1848fc49016fadf4e99d990aec0bd869d8a9d84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328773"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().languages("{id}")
    .buildRequest()
    .delete();

```