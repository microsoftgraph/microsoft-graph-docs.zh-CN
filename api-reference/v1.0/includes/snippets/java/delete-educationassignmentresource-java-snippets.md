---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53fb2fbe23e6dab192fad140a2f2b799b6a9e5ba414be9d3cb0db7d944e06839
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332622"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").resources("22002")
    .buildRequest()
    .delete();

```