---
title: loggedOnUser 资源类型
description: 在用户登录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 056fae8051b70f2146930c8a2a1ae9505c0ec679
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962091"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="b37e8-103">loggedOnUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="b37e8-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="b37e8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b37e8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b37e8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b37e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b37e8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b37e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b37e8-107">在用户登录</span><span class="sxs-lookup"><span data-stu-id="b37e8-107">Logged On User</span></span>
## <a name="properties"></a><span data-ttu-id="b37e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="b37e8-108">Properties</span></span>
|<span data-ttu-id="b37e8-109">属性</span><span class="sxs-lookup"><span data-stu-id="b37e8-109">Property</span></span>|<span data-ttu-id="b37e8-110">类型</span><span class="sxs-lookup"><span data-stu-id="b37e8-110">Type</span></span>|<span data-ttu-id="b37e8-111">Description</span><span class="sxs-lookup"><span data-stu-id="b37e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b37e8-112">userId</span><span class="sxs-lookup"><span data-stu-id="b37e8-112">userId</span></span>|<span data-ttu-id="b37e8-113">String</span><span class="sxs-lookup"><span data-stu-id="b37e8-113">String</span></span>|<span data-ttu-id="b37e8-114">用户 id</span><span class="sxs-lookup"><span data-stu-id="b37e8-114">User id</span></span>|
|<span data-ttu-id="b37e8-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="b37e8-115">lastLogOnDateTime</span></span>|<span data-ttu-id="b37e8-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b37e8-116">DateTimeOffset</span></span>|<span data-ttu-id="b37e8-117">当用户登录时的日期时间</span><span class="sxs-lookup"><span data-stu-id="b37e8-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="b37e8-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="b37e8-118">Relationships</span></span>
<span data-ttu-id="b37e8-119">无</span><span class="sxs-lookup"><span data-stu-id="b37e8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b37e8-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b37e8-120">JSON Representation</span></span>
<span data-ttu-id="b37e8-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b37e8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```





