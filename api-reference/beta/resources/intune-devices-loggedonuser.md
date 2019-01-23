---
title: loggedOnUser 资源类型
description: 在用户登录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ac0ca08c6d324836e4bb9dd9951fdfe742b8b5f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395193"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="d4dd2-103">loggedOnUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4dd2-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="d4dd2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d4dd2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4dd2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4dd2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4dd2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4dd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4dd2-107">在用户登录</span><span class="sxs-lookup"><span data-stu-id="d4dd2-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="d4dd2-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4dd2-108">Properties</span></span>
|<span data-ttu-id="d4dd2-109">属性</span><span class="sxs-lookup"><span data-stu-id="d4dd2-109">Property</span></span>|<span data-ttu-id="d4dd2-110">类型</span><span class="sxs-lookup"><span data-stu-id="d4dd2-110">Type</span></span>|<span data-ttu-id="d4dd2-111">说明</span><span class="sxs-lookup"><span data-stu-id="d4dd2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4dd2-112">userId</span><span class="sxs-lookup"><span data-stu-id="d4dd2-112">userId</span></span>|<span data-ttu-id="d4dd2-113">String</span><span class="sxs-lookup"><span data-stu-id="d4dd2-113">String</span></span>|<span data-ttu-id="d4dd2-114">用户 id</span><span class="sxs-lookup"><span data-stu-id="d4dd2-114">User id</span></span>|
|<span data-ttu-id="d4dd2-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="d4dd2-115">lastLogOnDateTime</span></span>|<span data-ttu-id="d4dd2-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4dd2-116">DateTimeOffset</span></span>|<span data-ttu-id="d4dd2-117">当用户登录时的日期时间</span><span class="sxs-lookup"><span data-stu-id="d4dd2-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4dd2-118">关系</span><span class="sxs-lookup"><span data-stu-id="d4dd2-118">Relationships</span></span>
<span data-ttu-id="d4dd2-119">无</span><span class="sxs-lookup"><span data-stu-id="d4dd2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4dd2-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4dd2-120">JSON Representation</span></span>
<span data-ttu-id="d4dd2-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4dd2-121">Here is a JSON representation of the resource.</span></span>
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




