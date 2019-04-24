---
title: iosWebContentFilterSpecificWebsitesAccess 资源类型
description: 表示 ios Web 内容筛选器设置类型, 该类型将 URL 书签安装到 iOS 内置浏览器中。 在课堂中, 教师希望学生通过在其 iOS 设备上配置的浏览器书签来导航网站, 而不能访问其他网站, 这是一个示例方案。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7d5b60af9a3b17923faac4dd0136ef6a9bc1591
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460469"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="fff4c-104">iosWebContentFilterSpecificWebsitesAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="fff4c-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="fff4c-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fff4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fff4c-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fff4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fff4c-107">表示 ios Web 内容筛选器设置类型, 该类型将 URL 书签安装到 iOS 内置浏览器中。</span><span class="sxs-lookup"><span data-stu-id="fff4c-107">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="fff4c-108">在课堂中, 教师希望学生通过在其 iOS 设备上配置的浏览器书签来导航网站, 而不能访问其他网站, 这是一个示例方案。</span><span class="sxs-lookup"><span data-stu-id="fff4c-108">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="fff4c-109">继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="fff4c-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fff4c-110">属性</span><span class="sxs-lookup"><span data-stu-id="fff4c-110">Properties</span></span>
|<span data-ttu-id="fff4c-111">属性</span><span class="sxs-lookup"><span data-stu-id="fff4c-111">Property</span></span>|<span data-ttu-id="fff4c-112">类型</span><span class="sxs-lookup"><span data-stu-id="fff4c-112">Type</span></span>|<span data-ttu-id="fff4c-113">说明</span><span class="sxs-lookup"><span data-stu-id="fff4c-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fff4c-114">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="fff4c-114">specificWebsitesOnly</span></span>|<span data-ttu-id="fff4c-115">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合</span><span class="sxs-lookup"><span data-stu-id="fff4c-115">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="fff4c-116">将安装到内置浏览器和用户的 URL 书签仅允许通过书签访问网站。</span><span class="sxs-lookup"><span data-stu-id="fff4c-116">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="fff4c-117">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="fff4c-117">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fff4c-118">websiteList</span><span class="sxs-lookup"><span data-stu-id="fff4c-118">websiteList</span></span>|<span data-ttu-id="fff4c-119">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合</span><span class="sxs-lookup"><span data-stu-id="fff4c-119">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="fff4c-120">将安装到内置浏览器和用户的 URL 书签仅允许通过书签访问网站。</span><span class="sxs-lookup"><span data-stu-id="fff4c-120">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="fff4c-121">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="fff4c-121">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fff4c-122">关系</span><span class="sxs-lookup"><span data-stu-id="fff4c-122">Relationships</span></span>
<span data-ttu-id="fff4c-123">无</span><span class="sxs-lookup"><span data-stu-id="fff4c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fff4c-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fff4c-124">JSON Representation</span></span>
<span data-ttu-id="fff4c-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fff4c-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```





