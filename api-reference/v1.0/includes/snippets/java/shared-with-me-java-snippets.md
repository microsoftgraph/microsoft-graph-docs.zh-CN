---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81354489104f71490f739c4b7262f059ff49e12b4ed3084d5b5dedf578ba03fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221431"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveSharedWithMeCollectionPage sharedWithMe = graphClient.me().drive()
    .sharedWithMe()
    .buildRequest()
    .get();

```