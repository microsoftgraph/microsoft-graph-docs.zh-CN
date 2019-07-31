---
title: educationPowerSchoolDataProvider 资源
description: 用于在将 PowerSchool 用作输入源时设置学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6a036435cb7cc1a4ef70960b09feb600fe7f39f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972591"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="3bd90-103">educationPowerSchoolDataProvider 资源</span><span class="sxs-lookup"><span data-stu-id="3bd90-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bd90-104">用于在将[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)用作输入源时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="3bd90-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="3bd90-105">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="3bd90-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3bd90-106">属性</span><span class="sxs-lookup"><span data-stu-id="3bd90-106">Properties</span></span>

| <span data-ttu-id="3bd90-107">属性</span><span class="sxs-lookup"><span data-stu-id="3bd90-107">Property</span></span> | <span data-ttu-id="3bd90-108">类型</span><span class="sxs-lookup"><span data-stu-id="3bd90-108">Type</span></span> | <span data-ttu-id="3bd90-109">说明</span><span class="sxs-lookup"><span data-stu-id="3bd90-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="3bd90-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="3bd90-110">**connectionUrl**</span></span> | <span data-ttu-id="3bd90-111">String</span><span class="sxs-lookup"><span data-stu-id="3bd90-111">String</span></span> | <span data-ttu-id="3bd90-112">指向 PowerSchool 实例的连接 URL。</span><span class="sxs-lookup"><span data-stu-id="3bd90-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="3bd90-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="3bd90-113">**clientId**</span></span> | <span data-ttu-id="3bd90-114">String</span><span class="sxs-lookup"><span data-stu-id="3bd90-114">String</span></span> |  <span data-ttu-id="3bd90-115">用于连接到 PowerSchool 的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="3bd90-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="3bd90-116">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="3bd90-116">**clientSecret**</span></span> | <span data-ttu-id="3bd90-117">String</span><span class="sxs-lookup"><span data-stu-id="3bd90-117">String</span></span> |  <span data-ttu-id="3bd90-118">用于对与 PowerSchool 实例的连接进行身份验证的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="3bd90-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="3bd90-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="3bd90-119">**schoolsIds**</span></span> | <span data-ttu-id="3bd90-120">String collection</span><span class="sxs-lookup"><span data-stu-id="3bd90-120">String collection</span></span> |  <span data-ttu-id="3bd90-121">要同步的学校列表。</span><span class="sxs-lookup"><span data-stu-id="3bd90-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="3bd90-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="3bd90-122">**schoolYear**</span></span> | <span data-ttu-id="3bd90-123">String</span><span class="sxs-lookup"><span data-stu-id="3bd90-123">String</span></span> |  <span data-ttu-id="3bd90-124">要同步的学校年。</span><span class="sxs-lookup"><span data-stu-id="3bd90-124">The school year to sync.</span></span> |
| <span data-ttu-id="3bd90-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="3bd90-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="3bd90-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bd90-126">Boolean</span></span> |  <span data-ttu-id="3bd90-127">指示源是否具有单个学生或教师的多个标识符。</span><span class="sxs-lookup"><span data-stu-id="3bd90-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="3bd90-128">**操作**</span><span class="sxs-lookup"><span data-stu-id="3bd90-128">**customizations**</span></span> | [<span data-ttu-id="3bd90-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="3bd90-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="3bd90-130">要应用于同步配置文件的可选自定义项。</span><span class="sxs-lookup"><span data-stu-id="3bd90-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3bd90-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3bd90-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
  "connectionUrl": "String",
  "clientId": "String",
  "clientSecret": "String",
  "schoolsIds": ["String"],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": "Boolean",
  "customizations": {"@odata.type": "microsoft.graph.educationSynchronizationCustomizations"}
}
```
