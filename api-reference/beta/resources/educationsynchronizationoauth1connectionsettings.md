---
title: educationSynchronizationOAuth1ConnectionSettings 资源
description: 当 OAuth1 要用于连接到的数据提供程序时，应使用此连接设置类型设置配置文件。
ms.openlocfilehash: 17bfbed14bf22d8b30d82766985d64595204d05b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047187"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="94425-103">educationSynchronizationOAuth1ConnectionSettings 资源</span><span class="sxs-lookup"><span data-stu-id="94425-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

> <span data-ttu-id="94425-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="94425-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94425-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="94425-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94425-106">当 OAuth1 要用于连接到的数据提供程序时，应使用此连接设置类型设置配置文件。</span><span class="sxs-lookup"><span data-stu-id="94425-106">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="94425-107">派生自[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="94425-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="94425-108">属性</span><span class="sxs-lookup"><span data-stu-id="94425-108">Properties</span></span>

<span data-ttu-id="94425-109">此类型不公开任何其他属性。</span><span class="sxs-lookup"><span data-stu-id="94425-109">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94425-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94425-110">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```
