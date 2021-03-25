---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48700c86035ce1a643d5ee2707013bb1bc2373f8
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209695"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002")
    .publish()
    .buildRequest()
    .post();

```