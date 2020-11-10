---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cd99c300e7b8d27ccfdbb7c5424bd0f1dc28d9b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972837"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookCategory outlookCategory = graphClient.me().outlook().masterCategories("de912e4d-c790-4da9-949c-ccd933aaa0f7")
    .buildRequest()
    .get();

```