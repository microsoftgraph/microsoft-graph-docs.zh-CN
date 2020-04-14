---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 11d227824bbced1789da25a0919371b54881a5ed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443728"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="7fa94-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="7fa94-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="7fa94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fa94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7fa94-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7fa94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fa94-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7fa94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fa94-107">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="7fa94-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="7fa94-108">属性</span><span class="sxs-lookup"><span data-stu-id="7fa94-108">Properties</span></span>
|<span data-ttu-id="7fa94-109">属性</span><span class="sxs-lookup"><span data-stu-id="7fa94-109">Property</span></span>|<span data-ttu-id="7fa94-110">类型</span><span class="sxs-lookup"><span data-stu-id="7fa94-110">Type</span></span>|<span data-ttu-id="7fa94-111">说明</span><span class="sxs-lookup"><span data-stu-id="7fa94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fa94-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="7fa94-112">subjectName</span></span>|<span data-ttu-id="7fa94-113">String</span><span class="sxs-lookup"><span data-stu-id="7fa94-113">String</span></span>|<span data-ttu-id="7fa94-114">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="7fa94-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="7fa94-115">description</span><span class="sxs-lookup"><span data-stu-id="7fa94-115">description</span></span>|<span data-ttu-id="7fa94-116">String</span><span class="sxs-lookup"><span data-stu-id="7fa94-116">String</span></span>|<span data-ttu-id="7fa94-117">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="7fa94-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="7fa94-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7fa94-118">expirationDateTime</span></span>|<span data-ttu-id="7fa94-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fa94-119">DateTimeOffset</span></span>|<span data-ttu-id="7fa94-120">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="7fa94-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="7fa94-121">证书</span><span class="sxs-lookup"><span data-stu-id="7fa94-121">certificate</span></span>|<span data-ttu-id="7fa94-122">Binary</span><span class="sxs-lookup"><span data-stu-id="7fa94-122">Binary</span></span>|<span data-ttu-id="7fa94-123">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="7fa94-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fa94-124">关系</span><span class="sxs-lookup"><span data-stu-id="7fa94-124">Relationships</span></span>
<span data-ttu-id="7fa94-125">无</span><span class="sxs-lookup"><span data-stu-id="7fa94-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fa94-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7fa94-126">JSON Representation</span></span>
<span data-ttu-id="7fa94-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fa94-127">Here is a JSON representation of the resource.</span></span>
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



