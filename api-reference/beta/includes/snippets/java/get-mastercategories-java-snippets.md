---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3aa4674d212bbc46351f93610d02bb5773b3e150
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979605"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOutlookCategoryCollectionPage masterCategories = graphClient.me().outlook().masterCategories()
    .buildRequest()
    .get();

```