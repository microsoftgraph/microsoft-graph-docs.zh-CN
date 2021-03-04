---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 196055f00bcc63cdab721e2f8fb31be6268401c2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433502"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().account("{id}")
    .buildRequest()
    .delete();

```