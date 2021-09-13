---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c12247182f0828a7382d1cde7e5f25dc49d75b74b21d9a18d6ada06810e5774
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104594"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.me().drive().root()
    .buildRequest()
    .get();

```