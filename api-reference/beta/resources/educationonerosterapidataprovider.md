---
title: educationOneRosterApiDataProvider 资源
description: 用于在将 OneRoster API 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ea02186b7d9bd7bed14c6ea5b46023da81814f07
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791060"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="88fab-103">educationOneRosterApiDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="88fab-103">educationOneRosterApiDataProvider resource</span></span>

<span data-ttu-id="88fab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88fab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88fab-105">用于在将[ONEROSTER API](https://www.imsglobal.org/activity/onerosterlis)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="88fab-105">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="88fab-106">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="88fab-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="88fab-107">属性</span><span class="sxs-lookup"><span data-stu-id="88fab-107">Properties</span></span>

| <span data-ttu-id="88fab-108">属性</span><span class="sxs-lookup"><span data-stu-id="88fab-108">Property</span></span>           | <span data-ttu-id="88fab-109">类型</span><span class="sxs-lookup"><span data-stu-id="88fab-109">Type</span></span>                                         | <span data-ttu-id="88fab-110">说明</span><span class="sxs-lookup"><span data-stu-id="88fab-110">Description</span></span>                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="88fab-111">connectionUrl</span><span class="sxs-lookup"><span data-stu-id="88fab-111">connectionUrl</span></span>      | <span data-ttu-id="88fab-112">String</span><span class="sxs-lookup"><span data-stu-id="88fab-112">String</span></span>                                       | <span data-ttu-id="88fab-113">指向 OneRoster 实例的连接 URL。</span><span class="sxs-lookup"><span data-stu-id="88fab-113">The connection URL to the OneRoster instance.</span></span>                                                         |
| <span data-ttu-id="88fab-114">providerName</span><span class="sxs-lookup"><span data-stu-id="88fab-114">providerName</span></span>       | <span data-ttu-id="88fab-115">String</span><span class="sxs-lookup"><span data-stu-id="88fab-115">String</span></span>                                       | <span data-ttu-id="88fab-116">由[OneRoster 规范][oneroster]定义的 OneRoster 服务提供程序名称。</span><span class="sxs-lookup"><span data-stu-id="88fab-116">The OneRoster Service Provider name as defined by the [OneRoster specification][oneroster].</span></span>           |
| <span data-ttu-id="88fab-117">schoolsIds</span><span class="sxs-lookup"><span data-stu-id="88fab-117">schoolsIds</span></span>         | <span data-ttu-id="88fab-118">String collection</span><span class="sxs-lookup"><span data-stu-id="88fab-118">String collection</span></span>                            | <span data-ttu-id="88fab-119">要同步的[学校/组织][orgs]的列表 `sourcedId` 。</span><span class="sxs-lookup"><span data-stu-id="88fab-119">The list of [School/Org][orgs] `sourcedId` to sync.</span></span>                                                   |
| <span data-ttu-id="88fab-120">termIds</span><span class="sxs-lookup"><span data-stu-id="88fab-120">termIds</span></span>            | <span data-ttu-id="88fab-121">String collection</span><span class="sxs-lookup"><span data-stu-id="88fab-121">String collection</span></span>                            | <span data-ttu-id="88fab-122">要同步的[学术会话][terms]的列表。</span><span class="sxs-lookup"><span data-stu-id="88fab-122">The list of [academic sessions][terms] to sync.</span></span>                                                       |
| <span data-ttu-id="88fab-123">connectionSettings</span><span class="sxs-lookup"><span data-stu-id="88fab-123">connectionSettings</span></span> | <span data-ttu-id="88fab-124">[educationSynchronizationConnectionSettings]</span><span class="sxs-lookup"><span data-stu-id="88fab-124">[educationSynchronizationConnectionSettings]</span></span> | <span data-ttu-id="88fab-125">OneRoster 实例的[oauth 1.0][onerosteroauth1]或[oauth 2.0][onerosteroauth2]设置。</span><span class="sxs-lookup"><span data-stu-id="88fab-125">The [OAuth 1.0][onerosteroauth1] or [OAuth 2.0][onerosteroauth2] settings for the OneRoster instance.</span></span> |
| <span data-ttu-id="88fab-126">操作</span><span class="sxs-lookup"><span data-stu-id="88fab-126">customizations</span></span>     | <span data-ttu-id="88fab-127">[educationSynchronizationCustomizations]）</span><span class="sxs-lookup"><span data-stu-id="88fab-127">[educationSynchronizationCustomizations])</span></span>    | <span data-ttu-id="88fab-128">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="88fab-128">Optional customization to be applied to the synchronization profile.</span></span>                                  |

> [!IMPORTANT]
> <span data-ttu-id="88fab-129">OneRoster 使用学术会议，而不是一年的时间来细分其数据。</span><span class="sxs-lookup"><span data-stu-id="88fab-129">OneRoster uses academic sessions rather than a single school year to segment their data.</span></span> <span data-ttu-id="88fab-130">此细分在学校数据同步 UI 中被抽象掉，而不是在此 API 中。</span><span class="sxs-lookup"><span data-stu-id="88fab-130">This segmentation is abstracted away within School Data Sync UI but not this API.</span></span> <span data-ttu-id="88fab-131">您需要调用 OneRoster `/terms` 终结点以获取学术会话 id 的集合，以便填充该 `termIds` 集合。</span><span class="sxs-lookup"><span data-stu-id="88fab-131">You will need to call the OneRoster `/terms` endpoint to get the collection of academic session IDs in order to populate the `termIds` collection.</span></span>

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md
[oneroster]: https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA
[onerosteroauth2]: educationsynchronizationoauth2clientcredentialsconnectionsettings.md
[onerosteroauth1]: educationsynchronizationoauth1connectionsettings.md
[terms]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452034
[orgs]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452016

## <a name="json-representation"></a><span data-ttu-id="88fab-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88fab-134">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
  "connectionUrl": "String",
  "providerName": "String",
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
  },
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneRosterApiDataProvider resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.settings"
  ]
}-->
