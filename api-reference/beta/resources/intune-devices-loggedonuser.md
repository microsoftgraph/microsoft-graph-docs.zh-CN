---
title: loggedOnUser 资源类型
description: 登录用户
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f953c176bf6163df0a53fc4996a29de060ebe191
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081277"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="b4806-103">loggedOnUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4806-103">loggedOnUser resource type</span></span>

<span data-ttu-id="b4806-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4806-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4806-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4806-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4806-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4806-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4806-107">登录用户</span><span class="sxs-lookup"><span data-stu-id="b4806-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="b4806-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4806-108">Properties</span></span>
|<span data-ttu-id="b4806-109">属性</span><span class="sxs-lookup"><span data-stu-id="b4806-109">Property</span></span>|<span data-ttu-id="b4806-110">类型</span><span class="sxs-lookup"><span data-stu-id="b4806-110">Type</span></span>|<span data-ttu-id="b4806-111">描述</span><span class="sxs-lookup"><span data-stu-id="b4806-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4806-112">userId</span><span class="sxs-lookup"><span data-stu-id="b4806-112">userId</span></span>|<span data-ttu-id="b4806-113">字符串</span><span class="sxs-lookup"><span data-stu-id="b4806-113">String</span></span>|<span data-ttu-id="b4806-114">用户 ID</span><span class="sxs-lookup"><span data-stu-id="b4806-114">User id</span></span>|
|<span data-ttu-id="b4806-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="b4806-115">lastLogOnDateTime</span></span>|<span data-ttu-id="b4806-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4806-116">DateTimeOffset</span></span>|<span data-ttu-id="b4806-117">用户登录的日期时间</span><span class="sxs-lookup"><span data-stu-id="b4806-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4806-118">关系</span><span class="sxs-lookup"><span data-stu-id="b4806-118">Relationships</span></span>
<span data-ttu-id="b4806-119">无</span><span class="sxs-lookup"><span data-stu-id="b4806-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4806-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4806-120">JSON Representation</span></span>
<span data-ttu-id="b4806-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4806-121">Here is a JSON representation of the resource.</span></span>
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






