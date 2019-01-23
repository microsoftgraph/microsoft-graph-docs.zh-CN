---
title: iosWebContentFilterSpecificWebsitesAccess 资源类型
description: 代表 iOS Web 内容筛选器设置类型，这将 URL 的书签安装到 iOS 内置浏览器。 示例方案是在课堂教师希望学生导航在浏览器书签其 iOS 的设备和不能访问其他网站上配置的网站。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 964ade2d2b46755fbba2903c6e9607340f60aedf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424761"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="36b55-104">iosWebContentFilterSpecificWebsitesAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="36b55-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="36b55-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="36b55-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="36b55-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="36b55-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36b55-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36b55-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36b55-108">代表 iOS Web 内容筛选器设置类型，这将 URL 的书签安装到 iOS 内置浏览器。</span><span class="sxs-lookup"><span data-stu-id="36b55-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="36b55-109">示例方案是在课堂教师希望学生导航在浏览器书签其 iOS 的设备和不能访问其他网站上配置的网站。</span><span class="sxs-lookup"><span data-stu-id="36b55-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="36b55-110">继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="36b55-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="36b55-111">属性</span><span class="sxs-lookup"><span data-stu-id="36b55-111">Properties</span></span>
|<span data-ttu-id="36b55-112">属性</span><span class="sxs-lookup"><span data-stu-id="36b55-112">Property</span></span>|<span data-ttu-id="36b55-113">类型</span><span class="sxs-lookup"><span data-stu-id="36b55-113">Type</span></span>|<span data-ttu-id="36b55-114">说明</span><span class="sxs-lookup"><span data-stu-id="36b55-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36b55-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="36b55-115">specificWebsitesOnly</span></span>|<span data-ttu-id="36b55-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合</span><span class="sxs-lookup"><span data-stu-id="36b55-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="36b55-117">将内置的浏览器和用户安装 URL 书签只允许通过书签访问网站。</span><span class="sxs-lookup"><span data-stu-id="36b55-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="36b55-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="36b55-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="36b55-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="36b55-119">websiteList</span></span>|<span data-ttu-id="36b55-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合</span><span class="sxs-lookup"><span data-stu-id="36b55-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="36b55-121">将内置的浏览器和用户安装 URL 书签只允许通过书签访问网站。</span><span class="sxs-lookup"><span data-stu-id="36b55-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="36b55-122">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="36b55-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36b55-123">关系</span><span class="sxs-lookup"><span data-stu-id="36b55-123">Relationships</span></span>
<span data-ttu-id="36b55-124">无</span><span class="sxs-lookup"><span data-stu-id="36b55-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36b55-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36b55-125">JSON Representation</span></span>
<span data-ttu-id="36b55-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36b55-126">Here is a JSON representation of the resource.</span></span>
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




