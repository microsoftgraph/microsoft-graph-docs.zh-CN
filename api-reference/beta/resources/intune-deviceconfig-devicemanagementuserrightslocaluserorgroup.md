---
title: deviceManagementUserRightsLocalUserOrGroup 资源类型
description: 表示一个本地用户或一组用于设置的用户权限的信息。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d795e2b259c71612b1d0720796b6ad76145bb36d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885736"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="b604e-103">deviceManagementUserRightsLocalUserOrGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="b604e-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="b604e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b604e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b604e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b604e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b604e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b604e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b604e-107">表示一个本地用户或一组用于设置的用户权限的信息。</span><span class="sxs-lookup"><span data-stu-id="b604e-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="b604e-108">属性</span><span class="sxs-lookup"><span data-stu-id="b604e-108">Properties</span></span>
|<span data-ttu-id="b604e-109">属性</span><span class="sxs-lookup"><span data-stu-id="b604e-109">Property</span></span>|<span data-ttu-id="b604e-110">类型</span><span class="sxs-lookup"><span data-stu-id="b604e-110">Type</span></span>|<span data-ttu-id="b604e-111">说明</span><span class="sxs-lookup"><span data-stu-id="b604e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b604e-112">name</span><span class="sxs-lookup"><span data-stu-id="b604e-112">name</span></span>|<span data-ttu-id="b604e-113">字符串</span><span class="sxs-lookup"><span data-stu-id="b604e-113">String</span></span>|<span data-ttu-id="b604e-114">此本地用户或组的名称。</span><span class="sxs-lookup"><span data-stu-id="b604e-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="b604e-115">说明</span><span class="sxs-lookup"><span data-stu-id="b604e-115">description</span></span>|<span data-ttu-id="b604e-116">字符串</span><span class="sxs-lookup"><span data-stu-id="b604e-116">String</span></span>|<span data-ttu-id="b604e-117">此本地用户或组的管理员的说明。</span><span class="sxs-lookup"><span data-stu-id="b604e-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="b604e-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="b604e-118">securityIdentifier</span></span>|<span data-ttu-id="b604e-119">字符串</span><span class="sxs-lookup"><span data-stu-id="b604e-119">String</span></span>|<span data-ttu-id="b604e-120">此本地用户或组的安全标识符 (例如 \* 1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="b604e-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="b604e-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="b604e-121">Relationships</span></span>
<span data-ttu-id="b604e-122">无</span><span class="sxs-lookup"><span data-stu-id="b604e-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b604e-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b604e-123">JSON Representation</span></span>
<span data-ttu-id="b604e-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b604e-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





