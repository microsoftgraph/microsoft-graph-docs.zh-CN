---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c358ea7578136b00c55549ad5d9e39f9c8810695
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968538"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/reports/getM365AppUserDetail(period='D7')/content", InputStream.class)
    .buildRequest()
    .get();

```