---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dcdd83346072a6f2946060a68064989b44ca3eb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940601"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="bb264-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb264-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="bb264-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb264-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb264-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb264-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb264-106">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="bb264-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="bb264-107">属性</span><span class="sxs-lookup"><span data-stu-id="bb264-107">Properties</span></span>
|<span data-ttu-id="bb264-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb264-108">Property</span></span>|<span data-ttu-id="bb264-109">类型</span><span class="sxs-lookup"><span data-stu-id="bb264-109">Type</span></span>|<span data-ttu-id="bb264-110">说明</span><span class="sxs-lookup"><span data-stu-id="bb264-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb264-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="bb264-111">subjectName</span></span>|<span data-ttu-id="bb264-112">String</span><span class="sxs-lookup"><span data-stu-id="bb264-112">String</span></span>|<span data-ttu-id="bb264-113">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="bb264-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="bb264-114">说明</span><span class="sxs-lookup"><span data-stu-id="bb264-114">description</span></span>|<span data-ttu-id="bb264-115">String</span><span class="sxs-lookup"><span data-stu-id="bb264-115">String</span></span>|<span data-ttu-id="bb264-116">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="bb264-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="bb264-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bb264-117">expirationDateTime</span></span>|<span data-ttu-id="bb264-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb264-118">DateTimeOffset</span></span>|<span data-ttu-id="bb264-119">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="bb264-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="bb264-120">证书</span><span class="sxs-lookup"><span data-stu-id="bb264-120">certificate</span></span>|<span data-ttu-id="bb264-121">Binary</span><span class="sxs-lookup"><span data-stu-id="bb264-121">Binary</span></span>|<span data-ttu-id="bb264-122">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="bb264-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb264-123">关系</span><span class="sxs-lookup"><span data-stu-id="bb264-123">Relationships</span></span>
<span data-ttu-id="bb264-124">无</span><span class="sxs-lookup"><span data-stu-id="bb264-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb264-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb264-125">JSON Representation</span></span>
<span data-ttu-id="bb264-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb264-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```




