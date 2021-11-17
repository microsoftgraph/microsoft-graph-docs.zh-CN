---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f35ec06fe40b8eeb5b8c405a302196c18351ebf4bc63499d8dea6fb7bf145b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278949"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InferenceClassificationOverrideCollectionPage overrides = graphClient.me().inferenceClassification().overrides()
    .buildRequest()
    .get();

```