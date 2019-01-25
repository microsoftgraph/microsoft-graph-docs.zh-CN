---
title: educationOneRosterApiDataProvider 资源
description: 用于 OneRoster API 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 55a3cd0e20f15c4b7d44bc7aebdc19f202e044f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527981"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="c1d92-103">educationOneRosterApiDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="c1d92-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1d92-104">用于[OneRoster API](https://www.imsglobal.org/activity/onerosterlis)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="c1d92-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="c1d92-105">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="c1d92-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c1d92-106">属性</span><span class="sxs-lookup"><span data-stu-id="c1d92-106">Properties</span></span>

| <span data-ttu-id="c1d92-107">属性</span><span class="sxs-lookup"><span data-stu-id="c1d92-107">Property</span></span> | <span data-ttu-id="c1d92-108">类型</span><span class="sxs-lookup"><span data-stu-id="c1d92-108">Type</span></span> | <span data-ttu-id="c1d92-109">说明</span><span class="sxs-lookup"><span data-stu-id="c1d92-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c1d92-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="c1d92-110">**connectionUrl**</span></span> | <span data-ttu-id="c1d92-111">String</span><span class="sxs-lookup"><span data-stu-id="c1d92-111">String</span></span> | <span data-ttu-id="c1d92-112">连接到 OneRoster 实例 URL。</span><span class="sxs-lookup"><span data-stu-id="c1d92-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="c1d92-113">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="c1d92-113">**schoolsIds**</span></span> | <span data-ttu-id="c1d92-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="c1d92-114">String collection</span></span> |  <span data-ttu-id="c1d92-115">学校 sourcedIds 同步的列表。</span><span class="sxs-lookup"><span data-stu-id="c1d92-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="c1d92-116">ProviderName</span><span class="sxs-lookup"><span data-stu-id="c1d92-116">**providerName**</span></span> | <span data-ttu-id="c1d92-117">String</span><span class="sxs-lookup"><span data-stu-id="c1d92-117">String</span></span> | <span data-ttu-id="c1d92-118">由[OneRoster 规范](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)定义 OneRoster 服务提供商的名称。</span><span class="sxs-lookup"><span data-stu-id="c1d92-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="c1d92-119">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="c1d92-119">**connectionSettings**</span></span> | [<span data-ttu-id="c1d92-120">microsoft.graph.educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="c1d92-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="c1d92-121">OneRoster 实例的连接设置。</span><span class="sxs-lookup"><span data-stu-id="c1d92-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="c1d92-122">应类型[microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)或[microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="c1d92-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="c1d92-123">**自定义项**</span><span class="sxs-lookup"><span data-stu-id="c1d92-123">**customizations**</span></span> | [<span data-ttu-id="c1d92-124">microsoft.graph.educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="c1d92-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="c1d92-125">可选自定义要应用于同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="c1d92-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1d92-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1d92-126">JSON representation</span></span>
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
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonerosterapidataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
