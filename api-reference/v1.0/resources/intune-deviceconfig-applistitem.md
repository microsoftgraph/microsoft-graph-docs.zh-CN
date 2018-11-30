---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
ms.openlocfilehash: c9b39b5fdee8bb503ef66f729a6ee478581a6391
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008245"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="63348-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="63348-103">appListItem resource type</span></span>

> <span data-ttu-id="63348-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="63348-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63348-105">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="63348-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="63348-106">属性</span><span class="sxs-lookup"><span data-stu-id="63348-106">Properties</span></span>
|<span data-ttu-id="63348-107">属性</span><span class="sxs-lookup"><span data-stu-id="63348-107">Property</span></span>|<span data-ttu-id="63348-108">类型</span><span class="sxs-lookup"><span data-stu-id="63348-108">Type</span></span>|<span data-ttu-id="63348-109">说明</span><span class="sxs-lookup"><span data-stu-id="63348-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63348-110">name</span><span class="sxs-lookup"><span data-stu-id="63348-110">name</span></span>|<span data-ttu-id="63348-111">String</span><span class="sxs-lookup"><span data-stu-id="63348-111">String</span></span>|<span data-ttu-id="63348-112">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="63348-112">The application name</span></span>|
|<span data-ttu-id="63348-113">publisher</span><span class="sxs-lookup"><span data-stu-id="63348-113">publisher</span></span>|<span data-ttu-id="63348-114">String</span><span class="sxs-lookup"><span data-stu-id="63348-114">String</span></span>|<span data-ttu-id="63348-115">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="63348-115">The publisher of the application</span></span>|
|<span data-ttu-id="63348-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="63348-116">appStoreUrl</span></span>|<span data-ttu-id="63348-117">String</span><span class="sxs-lookup"><span data-stu-id="63348-117">String</span></span>|<span data-ttu-id="63348-118">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="63348-118">The Store URL of the application</span></span>|
|<span data-ttu-id="63348-119">appId</span><span class="sxs-lookup"><span data-stu-id="63348-119">appId</span></span>|<span data-ttu-id="63348-120">String</span><span class="sxs-lookup"><span data-stu-id="63348-120">String</span></span>|<span data-ttu-id="63348-121">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="63348-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="63348-122">关系</span><span class="sxs-lookup"><span data-stu-id="63348-122">Relationships</span></span>
<span data-ttu-id="63348-123">无</span><span class="sxs-lookup"><span data-stu-id="63348-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="63348-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63348-124">JSON Representation</span></span>
<span data-ttu-id="63348-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63348-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



