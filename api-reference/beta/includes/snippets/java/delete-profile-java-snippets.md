---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5d3194af3be6c1d8b1bcd2620132738bef6f647
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969766"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile()
    .buildRequest()
    .delete();

```