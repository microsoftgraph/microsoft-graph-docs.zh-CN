---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa02b301dedbf58f5339439ae4afcba668f48914
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904936"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().todo().lists("AAMkADA1MTHgwAAA=").tasks("721a35e2-35e2-721a-e235-1a72e2351a72")
    .buildRequest()
    .delete();

```