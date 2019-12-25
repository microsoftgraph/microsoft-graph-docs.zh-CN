---
title: registryKeyState 资源类型
description: 包含有关与警报相关的注册表项更改的信息，以及更改了注册表项的过程。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e685bc281344f05a43e3c44b7df6bb6884185c63
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870129"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="66604-103">registryKeyState 资源类型</span><span class="sxs-lookup"><span data-stu-id="66604-103">registryKeyState resource type</span></span>

<span data-ttu-id="66604-104">包含有关与警报相关的注册表项更改的信息，以及更改了注册表项的过程。</span><span class="sxs-lookup"><span data-stu-id="66604-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="66604-105">属性</span><span class="sxs-lookup"><span data-stu-id="66604-105">Properties</span></span>

| <span data-ttu-id="66604-106">属性</span><span class="sxs-lookup"><span data-stu-id="66604-106">Property</span></span>     | <span data-ttu-id="66604-107">类型</span><span class="sxs-lookup"><span data-stu-id="66604-107">Type</span></span>        | <span data-ttu-id="66604-108">说明</span><span class="sxs-lookup"><span data-stu-id="66604-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66604-109">配置单元</span><span class="sxs-lookup"><span data-stu-id="66604-109">hive</span></span>|<span data-ttu-id="66604-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="66604-110">registryHive</span></span>|<span data-ttu-id="66604-111">[Windows 注册表配置单元](/windows/desktop/sysinfo/registry-hives)：</span><span class="sxs-lookup"><span data-stu-id="66604-111">A [Windows registry hive](/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="66604-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="66604-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="66604-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="66604-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="66604-114">HKEY_LOCAL_MACHINE \SAM</span><span class="sxs-lookup"><span data-stu-id="66604-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="66604-115">HKEY_LOCAL_MACHINE \Security</span><span class="sxs-lookup"><span data-stu-id="66604-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="66604-116">HKEY_LOCAL_MACHINE \Software</span><span class="sxs-lookup"><span data-stu-id="66604-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="66604-117">HKEY_LOCAL_MACHINE \System</span><span class="sxs-lookup"><span data-stu-id="66604-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="66604-118">HKEY_USERS\\。设置.</span><span class="sxs-lookup"><span data-stu-id="66604-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="66604-119">可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSecurity`、`localMachineSoftware`、`localMachineSystem`、`usersDefault`。</span><span class="sxs-lookup"><span data-stu-id="66604-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="66604-120">注册表项</span><span class="sxs-lookup"><span data-stu-id="66604-120">key</span></span>|<span data-ttu-id="66604-121">String</span><span class="sxs-lookup"><span data-stu-id="66604-121">String</span></span>|<span data-ttu-id="66604-122">当前（如已更改）的注册表项（不包括配置单元）。</span><span class="sxs-lookup"><span data-stu-id="66604-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="66604-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="66604-123">oldKey</span></span>|<span data-ttu-id="66604-124">String</span><span class="sxs-lookup"><span data-stu-id="66604-124">String</span></span>|<span data-ttu-id="66604-125">上一个（即 "更改前"）注册表项（不包括 HIVE）。</span><span class="sxs-lookup"><span data-stu-id="66604-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="66604-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="66604-126">oldValueData</span></span>|<span data-ttu-id="66604-127">String</span><span class="sxs-lookup"><span data-stu-id="66604-127">String</span></span>|<span data-ttu-id="66604-128">以前的（即更改之前）注册表项值数据（内容）。</span><span class="sxs-lookup"><span data-stu-id="66604-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="66604-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="66604-129">oldValueName</span></span>|<span data-ttu-id="66604-130">String</span><span class="sxs-lookup"><span data-stu-id="66604-130">String</span></span>|<span data-ttu-id="66604-131">以前的注册表项值名称（即 "更改前"）。</span><span class="sxs-lookup"><span data-stu-id="66604-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="66604-132">操作</span><span class="sxs-lookup"><span data-stu-id="66604-132">operation</span></span>|<span data-ttu-id="66604-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="66604-133">registryOperation</span></span>|<span data-ttu-id="66604-134">更改注册表项名称和/或值的操作。</span><span class="sxs-lookup"><span data-stu-id="66604-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="66604-135">可取值为：`unknown`、`create`、`modify`、`delete`。</span><span class="sxs-lookup"><span data-stu-id="66604-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="66604-136">processId</span><span class="sxs-lookup"><span data-stu-id="66604-136">processId</span></span>|<span data-ttu-id="66604-137">Int32</span><span class="sxs-lookup"><span data-stu-id="66604-137">Int32</span></span>|<span data-ttu-id="66604-138">修改注册表项的进程的进程 ID （PID）（进程详细信息将显示在警报的 "进程" 集合中）。</span><span class="sxs-lookup"><span data-stu-id="66604-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="66604-139">valueData</span><span class="sxs-lookup"><span data-stu-id="66604-139">valueData</span></span>|<span data-ttu-id="66604-140">String</span><span class="sxs-lookup"><span data-stu-id="66604-140">String</span></span>|<span data-ttu-id="66604-141">当前（如已更改）的注册表项值数据（内容）。</span><span class="sxs-lookup"><span data-stu-id="66604-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="66604-142">等值</span><span class="sxs-lookup"><span data-stu-id="66604-142">valueName</span></span>|<span data-ttu-id="66604-143">String</span><span class="sxs-lookup"><span data-stu-id="66604-143">String</span></span>|<span data-ttu-id="66604-144">当前（如已更改）的注册表项值名称</span><span class="sxs-lookup"><span data-stu-id="66604-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="66604-145">valueType</span><span class="sxs-lookup"><span data-stu-id="66604-145">valueType</span></span>|<span data-ttu-id="66604-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="66604-146">registryValueType</span></span>|[<span data-ttu-id="66604-147">注册表项值类型</span><span class="sxs-lookup"><span data-stu-id="66604-147">Registry key value type</span></span>](/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="66604-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="66604-148">REG_BINARY</span></span></li> <li><span data-ttu-id="66604-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="66604-149">REG_DWORD</span></span></li> <li><span data-ttu-id="66604-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="66604-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="66604-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="66604-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="66604-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="66604-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="66604-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="66604-153">REG_LINK</span></span></li> <li><span data-ttu-id="66604-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="66604-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="66604-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="66604-155">REG_NONE</span></span></li> <li><span data-ttu-id="66604-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="66604-156">REG_QWORD</span></span></li> <li><span data-ttu-id="66604-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="66604-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="66604-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="66604-158">REG_SZ</span></span></li></ul> <span data-ttu-id="66604-159">可取值为：`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz`。</span><span class="sxs-lookup"><span data-stu-id="66604-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66604-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66604-160">JSON representation</span></span>

<span data-ttu-id="66604-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66604-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
