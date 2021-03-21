---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3a94dfcc01ea4472b7e1cc85cbf9bc7265b89e5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973634"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookCategoryCollectionPage masterCategories = graphClient.me().outlook().masterCategories()
    .buildRequest()
    .get();

```