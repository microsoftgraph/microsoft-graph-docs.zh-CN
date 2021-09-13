---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7db594a4c261911fb691bc273673156225bab54f19f75037083e7d11460b4175
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104294"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .unmerge()
    .buildRequest()
    .post();

```