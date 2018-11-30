---
title: iosWebContentFilterSpecificWebsitesAccess 资源类型
description: 代表 iOS Web 内容筛选器设置类型，这将 URL 的书签安装到 iOS 内置浏览器。 示例方案是在课堂教师希望学生导航在浏览器书签其 iOS 的设备和不能访问其他网站上配置的网站。
ms.openlocfilehash: c5e23905ab9e5b692500544161fc052dd606da5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045769"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="a3f17-104">iosWebContentFilterSpecificWebsitesAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3f17-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

> <span data-ttu-id="a3f17-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a3f17-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3f17-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a3f17-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3f17-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a3f17-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3f17-108">代表 iOS Web 内容筛选器设置类型，这将 URL 的书签安装到 iOS 内置浏览器。</span><span class="sxs-lookup"><span data-stu-id="a3f17-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="a3f17-109">示例方案是在课堂教师希望学生导航在浏览器书签其 iOS 的设备和不能访问其他网站上配置的网站。</span><span class="sxs-lookup"><span data-stu-id="a3f17-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>

<span data-ttu-id="a3f17-110">继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="a3f17-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a3f17-111">属性</span><span class="sxs-lookup"><span data-stu-id="a3f17-111">Properties</span></span>
|<span data-ttu-id="a3f17-112">属性</span><span class="sxs-lookup"><span data-stu-id="a3f17-112">Property</span></span>|<span data-ttu-id="a3f17-113">类型</span><span class="sxs-lookup"><span data-stu-id="a3f17-113">Type</span></span>|<span data-ttu-id="a3f17-114">说明</span><span class="sxs-lookup"><span data-stu-id="a3f17-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3f17-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="a3f17-115">specificWebsitesOnly</span></span>|<span data-ttu-id="a3f17-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3f17-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="a3f17-117">将内置的浏览器和用户安装 URL 书签只允许通过书签访问网站。</span><span class="sxs-lookup"><span data-stu-id="a3f17-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="a3f17-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a3f17-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a3f17-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="a3f17-119">websiteList</span></span>|<span data-ttu-id="a3f17-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3f17-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="a3f17-121">将内置的浏览器和用户安装 URL 书签只允许通过书签访问网站。</span><span class="sxs-lookup"><span data-stu-id="a3f17-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="a3f17-122">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a3f17-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3f17-123">关系</span><span class="sxs-lookup"><span data-stu-id="a3f17-123">Relationships</span></span>
<span data-ttu-id="a3f17-124">无</span><span class="sxs-lookup"><span data-stu-id="a3f17-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a3f17-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3f17-125">JSON Representation</span></span>
<span data-ttu-id="a3f17-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3f17-126">Here is a JSON representation of the resource.</span></span>
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





