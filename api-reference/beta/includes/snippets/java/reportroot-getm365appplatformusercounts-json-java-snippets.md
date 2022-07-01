---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 066e15a4f87be02e44fe2249c0eb345e37784018
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577923"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/reports/getM365AppPlatformUserCounts(period='D7')", InputStream.class)
    .buildRequest()
    .get();

```