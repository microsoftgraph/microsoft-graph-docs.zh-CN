---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4ad031e97d6511280517ef1e9c3b30141c7125c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727181"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="ab6c2-103">windowsInformationProtectionDataRecoveryCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab6c2-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="ab6c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab6c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab6c2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab6c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab6c2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab6c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab6c2-107">Windows 信息保护 DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="ab6c2-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="ab6c2-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab6c2-108">Properties</span></span>
|<span data-ttu-id="ab6c2-109">属性</span><span class="sxs-lookup"><span data-stu-id="ab6c2-109">Property</span></span>|<span data-ttu-id="ab6c2-110">类型</span><span class="sxs-lookup"><span data-stu-id="ab6c2-110">Type</span></span>|<span data-ttu-id="ab6c2-111">说明</span><span class="sxs-lookup"><span data-stu-id="ab6c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab6c2-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="ab6c2-112">subjectName</span></span>|<span data-ttu-id="ab6c2-113">String</span><span class="sxs-lookup"><span data-stu-id="ab6c2-113">String</span></span>|<span data-ttu-id="ab6c2-114">数据恢复证书主题名称</span><span class="sxs-lookup"><span data-stu-id="ab6c2-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="ab6c2-115">说明</span><span class="sxs-lookup"><span data-stu-id="ab6c2-115">description</span></span>|<span data-ttu-id="ab6c2-116">String</span><span class="sxs-lookup"><span data-stu-id="ab6c2-116">String</span></span>|<span data-ttu-id="ab6c2-117">数据恢复证书说明</span><span class="sxs-lookup"><span data-stu-id="ab6c2-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="ab6c2-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ab6c2-118">expirationDateTime</span></span>|<span data-ttu-id="ab6c2-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab6c2-119">DateTimeOffset</span></span>|<span data-ttu-id="ab6c2-120">数据恢复证书过期日期/时间</span><span class="sxs-lookup"><span data-stu-id="ab6c2-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="ab6c2-121">证书</span><span class="sxs-lookup"><span data-stu-id="ab6c2-121">certificate</span></span>|<span data-ttu-id="ab6c2-122">Binary</span><span class="sxs-lookup"><span data-stu-id="ab6c2-122">Binary</span></span>|<span data-ttu-id="ab6c2-123">数据恢复证书</span><span class="sxs-lookup"><span data-stu-id="ab6c2-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab6c2-124">关系</span><span class="sxs-lookup"><span data-stu-id="ab6c2-124">Relationships</span></span>
<span data-ttu-id="ab6c2-125">无</span><span class="sxs-lookup"><span data-stu-id="ab6c2-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab6c2-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab6c2-126">JSON Representation</span></span>
<span data-ttu-id="ab6c2-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab6c2-127">Here is a JSON representation of the resource.</span></span>
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





