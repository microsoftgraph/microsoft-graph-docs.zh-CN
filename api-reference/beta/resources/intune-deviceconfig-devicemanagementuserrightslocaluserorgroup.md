---
title: deviceManagementUserRightsLocalUserOrGroup 资源类型
description: 表示一个本地用户或一组用于设置的用户权限的信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8a2cc0ff5b9e054398e7878b7d99619b59d109a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422059"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="43f9c-103">deviceManagementUserRightsLocalUserOrGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="43f9c-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="43f9c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="43f9c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43f9c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="43f9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43f9c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43f9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43f9c-107">表示一个本地用户或一组用于设置的用户权限的信息。</span><span class="sxs-lookup"><span data-stu-id="43f9c-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="43f9c-108">属性</span><span class="sxs-lookup"><span data-stu-id="43f9c-108">Properties</span></span>
|<span data-ttu-id="43f9c-109">属性</span><span class="sxs-lookup"><span data-stu-id="43f9c-109">Property</span></span>|<span data-ttu-id="43f9c-110">类型</span><span class="sxs-lookup"><span data-stu-id="43f9c-110">Type</span></span>|<span data-ttu-id="43f9c-111">说明</span><span class="sxs-lookup"><span data-stu-id="43f9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43f9c-112">name</span><span class="sxs-lookup"><span data-stu-id="43f9c-112">name</span></span>|<span data-ttu-id="43f9c-113">String</span><span class="sxs-lookup"><span data-stu-id="43f9c-113">String</span></span>|<span data-ttu-id="43f9c-114">此本地用户或组的名称。</span><span class="sxs-lookup"><span data-stu-id="43f9c-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="43f9c-115">说明</span><span class="sxs-lookup"><span data-stu-id="43f9c-115">description</span></span>|<span data-ttu-id="43f9c-116">String</span><span class="sxs-lookup"><span data-stu-id="43f9c-116">String</span></span>|<span data-ttu-id="43f9c-117">此本地用户或组的管理员的说明。</span><span class="sxs-lookup"><span data-stu-id="43f9c-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="43f9c-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="43f9c-118">securityIdentifier</span></span>|<span data-ttu-id="43f9c-119">String</span><span class="sxs-lookup"><span data-stu-id="43f9c-119">String</span></span>|<span data-ttu-id="43f9c-120">此本地用户或组的安全标识符 (例如 \* 1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="43f9c-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="43f9c-121">关系</span><span class="sxs-lookup"><span data-stu-id="43f9c-121">Relationships</span></span>
<span data-ttu-id="43f9c-122">无</span><span class="sxs-lookup"><span data-stu-id="43f9c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43f9c-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43f9c-123">JSON Representation</span></span>
<span data-ttu-id="43f9c-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43f9c-124">Here is a JSON representation of the resource.</span></span>
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




