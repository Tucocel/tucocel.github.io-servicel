<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SERVICEL MASTER — Panel de Control Técnico Profesional</title>
    
    <!-- CONFIGURACIÓN PWA PARA PANTALLA DE INICIO -->
    <link rel="manifest" href="data:application/json;base64,ewogICJuYW1lIjogIlNlcnZpY2VsIE1hc3RlciIsCiAgInNob3J0X25hbWUiOiAiU2VydmljZWwiLAogICJzdGFydF91cmwiOiAiLiIsCiAgImRpc3BsYXkiOiAic3RhbmRhbG9uZSIsCiAgImJhY2tncm91bmRfY29sb3IiOiAiIzAyMDYxNyIsCiAgInRoZW1lX2NvbG9yIjogIiNhODU1ZjciLAogICJpY29ucyI6IFsKICAgIHsKICAgICAgInNyYyI6ICJodHRwczovL2Nkbi1pY29ucy1wbmcuZmxhdGljb24uY29tLzUxMi8yOTA3LzI5MDc2MjgucG5nIiwKICAgICAgInNpemVzIjogIjUxMng1MTIiLAogICAgICAidHlwZSI6ICJpbWFnZS9wbmciCiAgICB9CiAgXQp9">
    
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght=400;500;600;700;800&display=swap');
        body { font-family: 'Plus Jakarta Sans', sans-serif; background-color: #020617; color: #f8fafc; }
        .no-scrollbar::-webkit-scrollbar { display: none; }
        .no-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }
        .glass-panel { background: rgba(15, 23, 42, 0.9); backdrop-filter: blur(16px); -webkit-backdrop-filter: blur(16px); }
    </style>
</head>
<body class="min-h-screen bg-slate-950 text-slate-100 overflow-x-hidden select-none flex flex-col justify-between">

    <!-- AVISO DE INSTALACIÓN PWA (UNA SOLA VEZ) -->
    <div id="pwa-install-banner" class="hidden fixed bottom-4 right-4 left-4 sm:left-auto sm:w-96 bg-slate-900 border border-purple-500/30 p-4 rounded-2xl shadow-2xl z-50 glass-panel">
        <div class="flex items-start gap-3">
            <div class="text-purple-400 text-2xl mt-1"><i class="fa-solid fa-mobile-screen-button"></i></div>
            <div class="space-y-1.5 flex-grow">
                <h4 class="text-sm font-extrabold text-white uppercase">Instalar en tu Pantalla</h4>
                <p class="text-xs text-slate-400 leading-relaxed">Añade Servicel Master a tu pantalla de inicio para entrar directo a facturar y reportar.</p>
                <div class="flex gap-2 justify-end">
                    <button onclick="window.svc_descartarInstalacionPWA()" class="text-xs font-bold text-slate-500 uppercase px-2 py-1">Descartar</button>
                    <button onclick="window.svc_dispararInstalacionPWA()" class="bg-purple-600 text-white text-xs font-black uppercase px-3 py-1.5 rounded-lg shadow-md">Instalar</button>
                </div>
            </div>
        </div>
    </div>

    <!-- CABECERA PRINCIPAL -->
    <header id="main-header" class="hidden border-b border-slate-900 bg-slate-900/40 py-4 px-4 sticky top-0 z-40 backdrop-blur-md">
        <div class="max-w-6xl mx-auto flex flex-col sm:flex-row justify-between items-center gap-4">
            <div class="flex items-center gap-3">
                <div class="w-12 h-12 bg-purple-600/10 border border-purple-500/30 rounded-xl flex items-center justify-center text-purple-400 text-2xl shadow-inner">
                    <i class="fa-solid fa-screwdriver-wrench"></i>
                </div>
                <div>
                    <h1 class="text-lg font-black tracking-tight text-white uppercase">SERVICEL MASTER</h1>
                    <span id="label-indicador-rol" class="text-[9px] bg-purple-950/40 px-2.5 py-0.5 border border-purple-500/20 text-purple-400 font-black tracking-widest uppercase block mt-1">ROL: DETECTANDO...</span>
                </div>
            </div>
            
            <!-- CONTENEDOR DE TASAS -->
            <div id="control-tasas-box" class="flex items-center gap-4 bg-slate-950 border border-slate-850 p-3 rounded-2xl text-xs font-bold font-mono">
                <div class="px-2 border-r border-slate-850">
                    <span class="block text-[8px] text-white uppercase font-sans mb-1">Tasa COP ($)</span>
                    <input type="number" id="cfg-tasa-cop" value="3600" onkeyup="window.svc_calcularConversionesAlVuelo()" class="w-16 bg-transparent text-amber-400 font-black focus:outline-none text-sm">
                </div>
                <div class="px-2">
                    <span class="block text-[8px] text-white uppercase font-sans mb-1">Tasa Bs vs COP</span>
                    <input type="number" id="cfg-tasa-bs" value="4" onkeyup="window.svc_calcularConversionesAlVuelo()" class="w-14 bg-transparent text-emerald-400 font-black focus:outline-none text-sm">
                </div>
            </div>
        </div>
    </header>

    <!-- PANTALLA: LOGIN DE ENTRADA -->
    <div id="contenedor-login" class="flex-grow flex items-center justify-center p-4">
        <div class="w-full max-w-md p-0.5 rounded-3xl bg-gradient-to-br from-purple-600 via-slate-800 to-indigo-600 shadow-2xl">
            <div class="glass-panel rounded-[22px] p-6 space-y-5">
                <div class="text-center space-y-2">
                    <div class="w-16 h-16 bg-purple-600/10 border border-purple-500/30 rounded-2xl flex items-center justify-center mx-auto text-purple-400 text-3xl shadow-inner"><i class="fa-solid fa-lock"></i></div>
                    <h2 class="font-black text-xl text-white tracking-tight uppercase">SERVICEL MASTER LOGIN</h2>
                    <p class="text-slate-400 text-xs">Coloque sus credenciales autorizadas de acceso.</p>
                </div>
                
                <!-- ADVERTENCIA OBLIGATORIA MANDATORIA -->
                <div class="bg-red-950/20 border border-red-500/30 p-4 rounded-2xl text-xs text-white font-bold leading-relaxed text-justify">
                    ⚠️ <b class="text-red-400 uppercase">DECLARACIÓN DE RESPONSABILIDAD:</b> El uso de esta plataforma es único y exclusivo. Usted es responsable de cada monto, repuesto y equipo registrado. Es una obligación ineludible indexar hasta el más mínimo trabajo de soporte técnico realizado en Servicel Master.
                </div>

                <div class="space-y-3 text-sm font-bold">
                    <input type="text" id="auth-user" placeholder="USUARIO ID" class="w-full bg-slate-950 border border-slate-800 px-4 py-3 rounded-xl text-white font-mono focus:outline-none focus:border-purple-500 uppercase">
                    <input type="password" id="auth-pass" placeholder="CONTRASEÑA MAESTRA" class="w-full bg-slate-950 border border-slate-800 px-4 py-3 rounded-xl text-white font-mono focus:outline-none focus:border-purple-500">
                    <button onclick="window.svc_ejecutarLoginGlobal()" class="w-full bg-gradient-to-r from-purple-600 to-indigo-600 text-white py-3.5 rounded-xl uppercase tracking-wider font-black shadow-md text-xs">Iniciar Sesión</button>
                </div>
            </div>
        </div>
    </div>

    <!-- PANTALLA: REGISTRO DE EXPEDIENTE (SOLO PRIMERA ENTRADA) -->
    <div id="contenedor-expediente-tecnico" class="hidden flex-grow flex items-center justify-center p-4">
        <div class="w-full max-w-lg p-0.5 rounded-3xl bg-gradient-to-br from-amber-500 to-purple-600 shadow-2xl">
            <div class="glass-panel rounded-[22px] p-6 space-y-4">
                <div class="text-center">
                    <span class="text-[9px] bg-amber-500/10 border border-amber-500/30 px-3 py-1 rounded-md text-amber-400 font-extrabold tracking-widest uppercase">FICHA LEGAL INALTERABLE</span>
                    <h2 class="font-black text-xl text-white mt-2 uppercase">Expediente de Personal</h2>
                    <p class="text-xs text-slate-400 mt-1">Por ley e instrucciones operativas de mostrador, complete sus datos legales antes de recibir cualquier equipo.</p>
                </div>
                <div class="space-y-3 text-xs font-bold text-slate-300">
                    <div>
                        <label class="text-[9px] text-white uppercase ml-1 block mb-1">Nombre Completo (Como figura en Cédula)</label>
                        <input type="text" id="exp-nombre" placeholder="Ej: MIGUEL GÓMEZ" class="w-full bg-slate-950 border border-slate-800 px-3.5 py-3 rounded-xl text-white uppercase focus:outline-none focus:border-amber-500">
                    </div>
                    <div class="grid grid-cols-2 gap-2">
                        <div>
                            <label class="text-[9px] text-white uppercase ml-1 block mb-1">Cédula de Identidad</label>
                            <input type="text" id="exp-cedula" placeholder="Ej: V-15888999" class="w-full bg-slate-950 border border-slate-800 px-3.5 py-3 rounded-xl text-white focus:outline-none focus:border-amber-500 font-mono">
                        </div>
                        <div>
                            <label class="text-[9px] text-white uppercase ml-1 block mb-1">WhatsApp Personal</label>
                            <input type="text" id="exp-whatsapp" placeholder="Ej: 04125554433" class="w-full bg-slate-950 border border-slate-800 px-3.5 py-3 rounded-xl text-white focus:outline-none focus:border-amber-500 font-mono">
                        </div>
                    </div>
                    <div>
                        <label class="text-[9px] text-white uppercase ml-1 block mb-1">Dirección de Domicilio Completa</label>
                        <input type="text" id="exp-direccion" placeholder="Ej: CALLE PRINCIPAL, SECTOR EL CENTRO" class="w-full bg-slate-950 border border-slate-800 px-3.5 py-3 rounded-xl text-white uppercase focus:outline-none focus:border-amber-500">
                    </div>
                    <button onclick="window.svc_guardarExpedienteTecnicoInalterable()" class="w-full bg-gradient-to-r from-amber-500 to-purple-600 text-white py-3.5 rounded-xl font-black uppercase tracking-wider text-xs">Guardar Expediente y Activar Consola</button>
                </div>
            </div>
        </div>
    </div>

    <!-- WORKSPACE CENTRAL CON PESTAÑAS 2X2 PARA MÓVIL -->
    <div id="contenedor-workspace" class="hidden max-w-6xl w-full mx-auto px-4 py-4 flex-grow flex flex-col gap-4">
        
        <!-- GRID DE PESTAÑAS 2X2 RESPONSIVO Y SEGURO -->
        <div id="workspace-tabs" class="grid grid-cols-2 sm:flex sm:flex-row gap-2 pb-3 no-imprimir">
            <button id="tab-btn-recepcion" onclick="window.svc_cambiarTab('recepcion')" class="w-full sm:w-auto bg-purple-600 text-white font-black text-center py-3 px-4 rounded-xl uppercase text-xs shadow flex items-center justify-center gap-2"><i class="fa-solid fa-cash-register text-sm"></i> Recepción</button>
            <button id="tab-btn-tecnicos" onclick="window.svc_cambiarTab('tecnicos')" class="w-full sm:w-auto bg-slate-900 text-slate-400 border border-slate-800 font-black text-center py-3 px-4 rounded-xl uppercase text-xs hidden flex items-center justify-center gap-2"><i class="fa-solid fa-users text-sm"></i> Técnicos</button>
            <button id="tab-btn-finanzas" onclick="window.svc_cambiarTab('finanzas')" class="w-full sm:w-auto bg-slate-900 text-slate-400 border border-slate-800 font-black text-center py-3 px-4 rounded-xl uppercase text-xs hidden flex items-center justify-center gap-2"><i class="fa-solid fa-vault text-sm"></i> Finanzas</button>
            <button id="tab-btn-garantias" onclick="window.svc_cambiarTab('garantias')" class="w-full sm:w-auto bg-slate-900 text-slate-400 border border-slate-800 font-black text-center py-3 px-4 rounded-xl uppercase text-xs hidden flex items-center justify-center gap-2"><i class="fa-solid fa-history text-sm"></i> Garantías</button>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-start w-full">
            
            <!-- HABITACIÓN 1: MOSTRADOR DE RECEPCIÓN -->
            <div id="tab-recepcion" class="lg:col-span-12 grid grid-cols-1 lg:grid-cols-12 gap-6 w-full">
                
                <!-- FORMULARIO REORGANIZADO Y GRANDE -->
                <div class="lg:col-span-6 bg-slate-900/60 border border-slate-800 rounded-3xl p-5 shadow-xl space-y-4">
                    <div class="border-b border-slate-800 pb-2 flex justify-between items-center">
                        <h3 class="text-sm font-black text-white uppercase tracking-widest flex items-center gap-1.5"><i class="fa-solid fa-square-plus text-purple-500"></i> Planilla de Entrada</h3>
                        <span class="text-[9px] bg-red-600/10 text-red-400 border border-red-500/20 px-2 py-0.5 rounded uppercase font-black">Control de Turno</span>
                    </div>

                    <div class="space-y-4 text-sm font-bold text-slate-300">
                        <!-- SELECTOR DE OPERADOR SEPARADO -->
                        <div class="bg-slate-950 p-3 border border-slate-850 rounded-xl flex items-center justify-between">
                            <span class="text-[10px] text-white uppercase font-sans">Operador que Recibe:</span>
                            <select id="form-operador" class="bg-slate-900 border border-slate-800 p-1.5 rounded-lg text-white font-black text-xs focus:outline-none uppercase"></select>
                        </div>

                        <div>
                            <label class="text-[10px] text-white uppercase ml-1 block mb-1">Nombre Completo del Cliente</label>
                            <input type="text" id="form-cliente" placeholder="Ej: CARLOS MENDOZA" class="w-full bg-slate-950 border border-slate-800 px-3.5 py-3 rounded-xl text-white uppercase focus:outline-none focus:border-purple-500 text-sm">
                        </div>
                        <div class="grid grid-cols-2 gap-2">
                            <div>
                                <label class="text-[10px] text-white uppercase ml-1 block mb-1">Cédula del Cliente</label>
                                <input type="text" id="form-cedula" placeholder="Ej: V-15888999" class="w-full bg-slate-950 border border-slate-800 px-3.5 py-3 rounded-xl text-white focus:outline-none font-mono text-sm">
                            </div>
                            <div>
                                <label class="text-[10px] text-white uppercase ml-1 block mb-1">WhatsApp de Contacto</label>
                                <input type="text" id="form-tlf" placeholder="Ej: 04125554433" class="w-full bg-slate-950 border border-slate-800 px-3.5 py-3 rounded-xl text-white focus:outline-none font-mono text-sm">
                            </div>
                        </div>
                        
                        <div class="grid grid-cols-2 gap-2 bg-slate-950/40 p-2 border border-slate-800 rounded-xl items-center">
                            <span class="text-[10px] text-white uppercase ml-1 block">Tipo de Mensajería:</span>
                            <select id="form-tipo-linea" class="bg-slate-900 border border-slate-800 p-1.5 rounded-lg text-white font-bold focus:outline-none text-xs">
                                <option value="WHATSAPP">🟢 WhatsApp Activo</option>
                                <option value="LLAMADA">📱 Solo Llamadas</option>
                            </select>
                        </div>

                        <div class="grid grid-cols-2 gap-2">
                            <div>
                                <label class="text-[10px] text-white uppercase ml-1 block mb-1">Marca y Modelo</label>
                                <input type="text" id="form-modelo" placeholder="Ej: REDMI NOTE 13" class="w-full bg-slate-950 border border-slate-800 px-3.5 py-3 rounded-xl text-white uppercase focus:outline-none text-sm">
                            </div>
                            <div>
                                <label class="text-[10px] text-white uppercase ml-1 block mb-1">Falla Reportada</label>
                                <input type="text" id="form-falla" placeholder="Ej: CAMBIO DE PANTALLA" class="w-full bg-slate-950 border border-slate-800 px-3.5 py-3 rounded-xl text-white uppercase focus:outline-none text-sm">
                            </div>
                        </div>

                        <!-- CARGA DE FOTO DE PATRÓN FÍSICO (RECIBO PAPEL) -->
                        <div class="bg-slate-950 p-4 rounded-2xl border border-slate-850 space-y-3">
                            <span class="text-[10px] text-purple-400 font-black uppercase block tracking-wider"><i class="fa-solid fa-camera mr-1"></i> Dibujo / Foto de Patrón en Papel</span>
                            <div class="grid grid-cols-2 gap-3 items-center">
                                <div>
                                    <label class="text-[9px] text-white uppercase block mb-1">Clave de Acceso</label>
                                    <input type="text" id="form-clave-manual" placeholder="Ej: 1234" class="w-full bg-slate-900 border border-slate-800 p-2 rounded-xl text-white font-mono text-center focus:outline-none uppercase text-sm">
                                </div>
                                <div class="flex flex-col items-center">
                                    <span class="text-[8px] text-slate-500 uppercase mb-1 block">Cargar Imagen</span>
                                    <label class="cursor-pointer bg-slate-900 hover:bg-slate-850 border border-slate-800 text-xs text-purple-400 font-black px-4 py-2.5 rounded-xl uppercase block text-center w-full shadow-md">
                                        <i class="fa-solid fa-upload mr-1"></i> Subir Foto
                                        <input type="file" id="form-foto-patron" accept="image/*" onchange="window.svc_procesarFotoPatronMostrador(this)" class="hidden">
                                    </label>
                                </div>
                            </div>
                            <!-- PREVIEW DE LA FOTO -->
                            <div id="wrapper-miniatura-patron" class="hidden flex justify-center bg-slate-900 p-2.5 rounded-xl border border-slate-850">
                                <img id="img-patron-preview" class="max-h-28 rounded-lg object-contain border border-slate-800 shadow-lg" src="" alt="Patrón">
                            </div>
                            <span class="text-[8px] text-slate-500 uppercase font-sans text-center block">"Aquí debes montar la foto del patrón del recibo del cliente"</span>
                        </div>

                        <!-- CHECKLIST DE ALMACENAMIENTO -->
                        <div class="bg-slate-950 p-4 rounded-2xl border border-slate-850 space-y-3">
                            <span class="text-[10px] text-purple-400 font-black uppercase block tracking-wider"><i class="fa-solid fa-clipboard-check mr-1"></i> Ficha Física de Resguardo</span>
                            <div class="grid grid-cols-3 gap-2 font-mono text-xs text-center">
                                <div class="bg-slate-900 p-2 rounded-xl border border-slate-800">
                                    <span class="block text-white text-[8px] uppercase mb-1">Chip SIM</span>
                                    <select id="chk-chip" class="w-full bg-slate-950 text-white rounded font-bold border border-slate-800 p-1 focus:outline-none text-xs"><option value="SÍ">SÍ</option><option value="NO" selected>NO</option></select>
                                </div>
                                <div class="bg-slate-900 p-2 rounded-xl border border-slate-800">
                                    <span class="block text-white text-[8px] uppercase mb-1">Memoria SD</span>
                                    <select id="chk-memoria" class="w-full bg-slate-950 text-white rounded font-bold border border-slate-800 p-1 focus:outline-none text-xs"><option value="SÍ">SÍ</option><option value="NO" selected>NO</option></select>
                                </div>
                                <div class="bg-slate-900 p-2 rounded-xl border border-slate-800">
                                    <span class="block text-white text-[8px] uppercase mb-1">Forro</span>
                                    <select id="chk-forro" class="w-full bg-slate-950 text-white rounded font-bold border border-slate-800 p-1 focus:outline-none text-xs"><option value="SÍ" selected>SÍ</option><option value="NO">NO</option></select>
                                </div>
                            </div>
                            <textarea id="form-detalles-manual" placeholder="Detalle manual de condiciones físicas o ralladuras..." rows="2" class="w-full bg-slate-900 border border-slate-800 p-2.5 rounded-xl text-white font-medium focus:outline-none uppercase text-xs"></textarea>
                        </div>

                        <!-- SECCIÓN MONTO Y ABONO CON SALDOS PENDIENTES AUTOMÁTICOS -->
                        <div class="bg-slate-950 p-4 rounded-2xl border border-slate-855 space-y-3">
                            <span class="text-[10px] text-amber-400 font-black uppercase block tracking-wider"><i class="fa-solid fa-coins mr-1"></i> Control de Cobro y Abono</span>
                            <div class="grid grid-cols-2 gap-3">
                                <div>
                                    <label class="text-[9px] text-white uppercase block mb-1">Recibe en</label>
                                    <select id="form-moneda-base" onchange="window.svc_conmutarMonedaMostrador()" class="w-full bg-slate-900 border border-slate-800 p-2.5 rounded-xl text-white text-xs focus:outline-none font-bold">
                                        <option value="USD">Dólares ($)</option>
                                        <option value="COP">Pesos (COP)</option>
                                    </select>
                                </div>
                                <div>
                                    <label class="text-[9px] text-white uppercase block mb-1">Monto Total</label>
                                    <input type="number" id="form-monto" placeholder="0.00" onkeyup="window.svc_calcularConversionesAlVuelo()" class="w-full bg-slate-900 border border-purple-500/40 px-3.5 py-2 rounded-xl text-white text-center font-mono text-sm font-black focus:outline-none">
                                </div>
                            </div>
                            
                            <!-- REGISTRO DEL MONTO ABONADO -->
                            <div class="grid grid-cols-2 gap-3 pt-2 border-t border-slate-900/60">
                                <div>
                                    <label class="text-[9px] text-white uppercase block mb-1">Monto Abonado</label>
                                    <input type="number" id="form-abono" value="0" onkeyup="window.svc_calcularConversionesAlVuelo()" class="w-full bg-slate-900 border border-emerald-500/30 px-3.5 py-2 rounded-xl text-white text-center font-mono text-sm font-black focus:outline-none">
                                </div>
                                <div class="flex flex-col justify-center items-center">
                                    <span class="text-[8px] text-red-400 font-extrabold uppercase tracking-wide">Pendiente de Cobro</span>
                                    <span id="lbl-display-pendiente" class="text-red-500 text-sm font-black font-mono">0.00 USD</span>
                                </div>
                            </div>

                            <div class="grid grid-cols-2 gap-2 font-mono text-[10px] text-center pt-2 border-t border-slate-900">
                                <div class="bg-slate-900/60 p-2 rounded-xl border border-slate-850"><span class="block text-[8px] text-white uppercase font-sans mb-1">Total en Pesos</span><b id="lbl-display-pesos" class="text-amber-400 block font-black text-sm">0 COP</b></div>
                                <div class="bg-slate-900/60 p-2 rounded-xl border border-slate-850"><span class="block text-[8px] text-white uppercase font-sans mb-1">Total en Bolívares</span><b id="lbl-display-bolivares" class="text-emerald-400 block font-black text-sm">0.00 Bs</b></div>
                            </div>
                        </div>

                        <div class="grid grid-cols-2 gap-2">
                            <div class="bg-slate-950 border border-slate-850 rounded-xl p-2 flex items-center justify-between text-xs">
                                <span class="text-[9px] text-white uppercase font-sans">Canal:</span>
                                <select id="form-tipo-op" class="bg-slate-900 border border-slate-800 p-1.5 rounded-lg text-white font-bold focus:outline-none"><option value="SERVICIO">🛠️ Servicio</option><option value="VENTA">🛍️ Venta</option></select>
                            </div>
                            <button onclick="window.svc_guardarComandaWorkspace()" class="w-full bg-gradient-to-r from-purple-600 to-indigo-600 text-white text-xs font-black py-3 rounded-xl uppercase tracking-wider shadow">Guardar Registro</button>
                        </div>
                    </div>
                </div>

                <!-- VISOR FIJO INALTERABLE -->
                <div class="lg:col-span-6 space-y-4">
                    <div class="bg-slate-900/60 border border-slate-800 rounded-3xl p-5 shadow-xl space-y-4">
                        <h3 class="text-sm font-black text-white uppercase tracking-widest border-b border-slate-800 pb-2 flex items-center gap-1.5"><i class="fa-solid fa-eye text-blue-400"></i> Última Recepción Registrada</h3>
                        <div id="wrapper-ultimo-visor" class="p-4 bg-slate-950 rounded-2xl border border-slate-850 text-sm space-y-3">
                            <p class="text-slate-500 text-center italic py-20">Ningún registro procesado en esta sesión.</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- HABITACIÓN 2: GESTIÓN DE TÉCNICOS Y EXPEDIENTES -->
            <div id="tab-tecnicos" class="lg:col-span-12 hidden w-full grid grid-cols-1 md:grid-cols-12 gap-6">
                
                <!-- CREAR NUEVO PERFIL -->
                <div class="md:col-span-5 bg-slate-900 p-5 rounded-3xl border border-slate-800 space-y-4">
                    <h3 class="text-sm font-black text-white uppercase tracking-wider border-b border-slate-800 pb-2 flex items-center gap-2"><i class="fa-solid fa-user-plus text-purple-500"></i> Crear Perfil para Técnico</h3>
                    <div class="space-y-3 text-sm font-bold text-slate-300">
                        <div>
                            <label class="text-[9px] text-white uppercase ml-1 block mb-1">Nombre Completo</label>
                            <input type="text" id="adm-tec-nombre" placeholder="Ej: Nelson" class="w-full bg-slate-950 border border-slate-800 px-3 py-2.5 rounded-xl text-white focus:outline-none">
                        </div>
                        <div class="grid grid-cols-2 gap-2">
                            <div>
                                <label class="text-[9px] text-white uppercase ml-1 block mb-1">Asignar Usuario ID</label>
                                <input type="text" id="adm-tec-user" placeholder="Ej: nelson" class="w-full bg-slate-950 border border-slate-800 px-3 py-2.5 rounded-xl text-white font-mono focus:outline-none uppercase">
                            </div>
                            <div>
                                <label class="text-[9px] text-white uppercase ml-1 block mb-1">Asignar Contraseña</label>
                                <input type="text" id="adm-tec-pass" placeholder="Ej: pass123" class="w-full bg-slate-950 border border-slate-800 px-3 py-2.5 rounded-xl text-white font-mono focus:outline-none">
                            </div>
                        </div>
                        <div class="grid grid-cols-2 gap-2">
                            <div>
                                <label class="text-[9px] text-white uppercase ml-1 block mb-1">WhatsApp de Envío</label>
                                <input type="text" id="adm-tec-whatsapp" placeholder="Ej: 58424000000" class="w-full bg-slate-950 border border-slate-800 px-3 py-2.5 rounded-xl text-white font-mono focus:outline-none">
                            </div>
                            <div>
                                <label class="text-[9px] text-white uppercase ml-1 block mb-1">% de Comisión</label>
                                <input type="number" id="adm-tec-comision" value="50" class="w-full bg-slate-950 border border-slate-800 px-3 py-2.5 rounded-xl text-white text-center font-mono focus:outline-none">
                            </div>
                        </div>
                        <button onclick="window.svc_crearNuevoPerfilTecnicoMaster()" class="w-full bg-purple-600 text-white text-xs py-3 rounded-xl font-black uppercase tracking-wider shadow">Registrar Colaborador</button>
                    </div>
                </div>

                <!-- EXPEDIENTES GUARDADOS -->
                <div class="md:col-span-7 bg-slate-900 p-5 rounded-3xl border border-slate-800 space-y-4">
                    <h3 class="text-sm font-black text-white uppercase tracking-wider border-b border-slate-800 pb-2 flex items-center gap-2"><i class="fa-solid fa-folder-open text-amber-500"></i> Expedientes y Fichas de Técnicos</h3>
                    <div id="wrapper-fichas-tecnicos-grid" class="grid grid-cols-1 sm:grid-cols-2 gap-3 max-h-96 overflow-y-auto no-scrollbar pr-1"></div>
                </div>
            </div>

            <!-- HABITACIÓN 3: BÓVEDA DE FINANZAS -->
            <div id="tab-finanzas" class="lg:col-span-12 hidden w-full space-y-6">
                <!-- BALANCES MONETARIOS -->
                <div id="wrapper-fines-totales-moneda" class="grid grid-cols-1 sm:grid-cols-3 gap-3"></div>
                
                <div class="bg-slate-900 border border-slate-800 p-5 rounded-3xl grid grid-cols-1 md:grid-cols-12 gap-6">
                    <div class="md:col-span-7 space-y-3">
                        <h3 class="text-white font-black text-sm uppercase tracking-wider border-b border-slate-800 pb-2">Comandas Activas en el Turno</h3>
                        <div id="wrapper-comandas-finanzas-grid" class="space-y-2 max-h-80 overflow-y-auto no-scrollbar text-xs text-slate-300"></div>
                    </div>
                    <div class="md:col-span-5 bg-slate-950 border border-slate-850 p-4 rounded-2xl space-y-4">
                        <div class="flex justify-between items-center border-b border-slate-900 pb-2">
                            <h3 class="text-purple-400 font-black text-xs uppercase">Rendimiento Técnico</h3>
                            <button onclick="window.svc_ejecutarCierreSemanalTotalHistorico()" class="bg-red-600/10 border border-red-500/20 text-red-400 text-[10px] font-black px-3 py-1.5 rounded-xl uppercase">Cierre Semanal</button>
                        </div>
                        <div class="grid grid-cols-2 gap-2 text-center font-mono text-xs">
                            <div class="bg-slate-900 p-2.5 rounded-xl border border-slate-850"><span class="block text-[8px] text-white uppercase font-sans mb-1">Nóminas Totales</span><b id="lbl-total-nominas" class="text-purple-400 text-sm font-black">$0.00</b></div>
                            <div class="bg-slate-900 p-2.5 rounded-xl border border-slate-850"><span class="block text-[8px] text-white uppercase font-sans mb-1">Caja Neta Servicel</span><b id="lbl-total-caja-neta" class="text-amber-400 text-sm font-black">$0.00</b></div>
                        </div>
                        <div class="border-t border-slate-900 pt-3">
                            <label class="text-[9px] text-white font-bold uppercase block mb-1">Adelanto Semanal de Caja ($)</label>
                            <div class="flex gap-1.5">
                                <select id="form-vale-tecnico-dest" class="bg-slate-900 border border-slate-800 p-2 rounded-xl font-bold text-xs text-white uppercase focus:outline-none"></select>
                                <input type="number" id="form-vale-monto" placeholder="Monto USD" class="w-full bg-slate-900 border border-slate-800 p-2 rounded-xl font-bold text-center text-xs text-white focus:outline-none">
                                <button onclick="window.svc_registrarValeColaborador()" class="bg-purple-600 text-white font-black px-4 rounded-xl text-xs uppercase tracking-wider">Abonar</button>
                            </div>
                        </div>
                        <div id="wrapper-vales-turno-grid" class="space-y-1 font-mono text-[9px] text-slate-500 max-h-24 overflow-y-auto no-scrollbar"></div>
                    </div>
                </div>
            </div>

            <!-- HABITACIÓN 4: RASTREADOR DE GARANTÍAS -->
            <div id="tab-garantias" class="lg:col-span-12 hidden w-full space-y-4">
                <div class="bg-slate-900 border border-slate-800 p-5 rounded-3xl space-y-4">
                    <div class="bg-slate-950 p-3 rounded-2xl border border-slate-855 space-y-2">
                        <span class="text-[9px] text-white uppercase tracking-wider font-mono block font-bold"><i class="fa-solid fa-history mr-1"></i> Rastreador General por Cédula / Orden</span>
                        <div class="flex gap-1.5">
                            <input type="text" id="search-criterio" onkeyup="window.svc_filtrarComandasBuscador()" placeholder="Escriba Cédula, Nombre del Cliente o Número de Orden..." class="w-full bg-slate-900 border border-slate-800 p-2.5 rounded-xl text-xs font-medium focus:outline-none">
                            <button onclick="document.getElementById('search-criterio').value=''; window.svc_filtrarComandasBuscador();" class="bg-slate-900 text-slate-400 border border-slate-800 text-xs px-4 rounded-xl uppercase">Limpiar</button>
                        </div>
                    </div>
                    <div id="wrapper-comandas-garantias-grid" class="space-y-2 max-h-96 overflow-y-auto no-scrollbar text-xs text-slate-300"></div>
                </div>
            </div>

        </div>
    </div>

    <footer class="bg-slate-900/20 border-t border-slate-900/60 py-3 text-center text-slate-500 font-mono text-[8px] tracking-widest">
        🔒 SERVICEL MASTER PLENARY PLATFORMS — REGISTRADA 2026
    </footer>

    <!-- ENGINE CORE FIREBASE INTEGRADO -->
    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/10.8.0/firebase-app.js";
        import { getFirestore, doc, setDoc, getDoc } from "https://www.gstatic.com/firebasejs/10.8.0/firebase-firestore.js";

        const firebaseConfig = {
          apiKey: "AIzaSyDytP_5UQyyRUT7wPC2bDIYz5t70z_pQV4",
          authDomain: "tucocel-vitrina.firebaseapp.com",
          projectId: "tucocel-vitrina",
          storageBucket: "tucocel-vitrina.firebasestorage.app"
        };

        const app = initializeApp(firebaseConfig);
        const db = getFirestore(app);

        // Variables de Control Interno
        let svc_comandasGlobal = [];
        let svc_valesGlobal = [];
        let svc_cierresGlobal = [];
        let svc_tecnicosPerfiles = [];
        let svc_fotoPatronBase64 = "";
        let rolDeSesionActiva = "BLOQUEADO";
        let usuarioSesionActivo = "";
        let deferredPrompt;

        // --- SISTEMA PWA SILENCIOSO INTELIGENTE ---
        window.addEventListener('beforeinstallprompt', (e) => {
            e.preventDefault();
            deferredPrompt = e;
            const descartado = localStorage.getItem('servicel_pwa_descartado');
            if(!descartado) {
                document.getElementById('pwa-install-banner').classList.remove('hidden');
            }
        });

        window.svc_dispararInstalacionPWA = async function() {
            if(!deferredPrompt) return;
            deferredPrompt.prompt();
            const { outcome } = await deferredPrompt.userChoice;
            if(outcome === 'accepted') {
                localStorage.setItem('servicel_pwa_descartado', 'true');
            }
            document.getElementById('pwa-install-banner').classList.add('hidden');
        };

        window.svc_descartarInstalacionPWA = function() {
            localStorage.setItem('servicel_pwa_descartado', 'true');
            document.getElementById('pwa-install-banner').classList.add('hidden');
        };

        // --- MANEJO DE FOTO DE PATRÓN ---
        window.svc_procesarFotoPatronMostrador = function(input) {
            const file = input.files[0];
            if(!file) return;
            const reader = new FileReader();
            reader.onload = function(e) {
                svc_fotoPatronBase64 = e.target.result;
                document.getElementById('img-patron-preview').src = svc_fotoPatronBase64;
                document.getElementById('wrapper-miniatura-patron').classList.remove('hidden');
            };
            reader.readAsDataURL(file);
        };

        // --- CONMUTADOR DE MONEDA ---
        window.svc_conmutarMonedaMostrador = function() {
            document.getElementById('form-monto').value = "";
            document.getElementById('form-abono').value = "0";
            document.getElementById('lbl-display-pesos').innerText = "0 COP";
            document.getElementById('lbl-display-bolivares').innerText = "0.00 Bs";
            document.getElementById('lbl-display-pendiente').innerText = "0.00 USD";
        };

        // --- MATEMÁTICA EXACTA DE ROBERT ($120 * 3600 = 432,000 COP / 4 = 108,000 COP) ---
        window.svc_calcularConversionesAlVuelo = function() {
            const moneda = document.getElementById('form-moneda-base').value;
            const monto = parseFloat(document.getElementById('form-monto').value) || 0;
            const abono = parseFloat(document.getElementById('form-abono').value) || 0;
            const tCOP = parseFloat(document.getElementById('cfg-tasa-cop').value) || 3600;
            const tBs = parseFloat(document.getElementById('cfg-tasa-bs').value) || 4;

            const lblCOP = document.getElementById('lbl-display-pesos');
            const lblBs = document.getElementById('lbl-display-bolivares');
            const lblPendiente = document.getElementById('lbl-display-pendiente');

            const saldoRestante = Math.max(0, monto - abono);

            if(monto <= 0) { 
                lblCOP.innerText = "0 COP"; 
                lblBs.innerText = "0.00 Bs"; 
                lblPendiente.innerText = "0.00 USD";
                return; 
            }

            if(moneda === "USD") {
                let totalPesos = monto * tCOP;
                let totalBs = totalPesos / tBs;
                lblCOP.innerText = `${Math.round(totalPesos).toLocaleString()} COP`;
                lblBs.innerText = `${totalBs.toFixed(2)} Bs`;
                lblPendiente.innerText = `$${saldoRestante.toFixed(2)} USD`;
            } else if(moneda === "COP") {
                let totalBs = monto / tBs;
                lblCOP.innerText = `${Math.round(monto).toLocaleString()} COP`;
                lblBs.innerText = `${totalBs.toFixed(2)} Bs`;
                
                let totalPendienteCOP = saldoRestante;
                lblPendiente.innerText = `${Math.round(totalPendienteCOP).toLocaleString()} COP`;
            }
        };

        // --- SISTEMA DE CREDENCIALES ---
        window.svc_ejecutarLoginGlobal = async function() {
            try {
                const user = document.getElementById('auth-user').value.trim().toLowerCase();
                const pass = document.getElementById('auth-pass').value.trim();

                const docSnapTecs = await getDoc(doc(db, "tcl_servicell_independent", "tecnicos_perfiles"));
                svc_tecnicosPerfiles = docSnapTecs.exists() ? docSnapTecs.data().perfiles || [] : [];

                if(user === "tucocel" && pass === "Razu2020.") {
                    rolDeSesionActiva = "MASTER";
                    usuarioSesionActivo = "MASTER";
                    document.getElementById('label-indicador-rol').innerText = "SESIÓN: MÁSTER SUPREMO CONTROLES";
                    document.getElementById('label-indicador-rol').className = "text-[9px] bg-blue-950/40 px-2.5 py-0.5 border border-blue-500/20 text-blue-400 font-black tracking-widest uppercase block mt-1";
                    
                    document.getElementById('tab-btn-tecnicos').classList.remove('hidden');
                    document.getElementById('tab-btn-finanzas').classList.remove('hidden');
                    document.getElementById('tab-btn-garantias').classList.remove('hidden');

                    window.svc_desbloquearWORKSPACE();
                } else {
                    const tecMatch = svc_tecnicosPerfiles.find(t => t.user.toLowerCase() === user && t.pass === pass);
                    if(tecMatch) {
                        rolDeSesionActiva = "TECNICO";
                        usuarioSesionActivo = tecMatch.user;
                        document.getElementById('label-indicador-rol').innerText = `SESIÓN: TÉCNICO (${tecMatch.nombre.toUpperCase()})`;
                        document.getElementById('label-indicador-rol').className = "text-[9px] bg-purple-950/40 px-2.5 py-0.5 border border-purple-500/20 text-purple-400 font-black tracking-widest uppercase block mt-1";
                        document.getElementById('control-tasas-box').classList.add('hidden');

                        const docExp = await getDoc(doc(db, "tcl_servicell_independent", `expediente_${usuarioSesionActivo}`));
                        if(!docExp.exists()) {
                            document.getElementById('contenedor-login').classList.add('hidden');
                            document.getElementById('contenedor-expediente-tecnico').classList.remove('hidden');
                        } else {
                            window.svc_desbloquearWORKSPACE();
                        }
                    } else {
                        alert("❌ Credenciales incorrectas.");
                    }
                }
            } catch(e) {}
        };

        window.svc_guardarExpedienteTecnicoInalterable = async function() {
            const nombre = document.getElementById('exp-nombre').value.trim().toUpperCase();
            const cedula = document.getElementById('exp-cedula').value.trim();
            const whatsapp = document.getElementById('exp-whatsapp').value.trim();
            const direccion = document.getElementById('exp-direccion').value.trim().toUpperCase();

            if(!nombre || !cedula || !whatsapp || !direccion) return alert("⚠️ Todos los campos son obligatorios por ley.");

            await setDoc(doc(db, "tcl_servicell_independent", `expediente_${usuarioSesionActivo}`), {
                nombre, cedula, whatsapp, direccion, fechaAlta: new Date().toLocaleDateString()
            });

            document.getElementById('contenedor-expediente-tecnico').classList.add('hidden');
            window.svc_desbloquearWORKSPACE();
        };

        window.svc_desbloquearWORKSPACE = async function() {
            document.getElementById('contenedor-login').classList.add('hidden');
            document.getElementById('main-header').classList.remove('hidden');
            document.getElementById('contenedor-workspace').classList.remove('hidden');
            await window.svc_descargarServidorCentral();
        };

        window.svc_descargarServidorCentral = async function() {
            try {
                const docSnap = await getDoc(doc(db, "tcl_servicell_independent", "comandas_data"));
                if(docSnap.exists()) {
                    svc_comandasGlobal = docSnap.data().comandas || [];
                    svc_valesGlobal = docSnap.data().vales || [];
                    svc_cierresGlobal = docSnap.data().historico || [];
                }
                window.svc_renderizarEcosistema();
            } catch(e) {}
        };

        window.svc_cambiarTab = function(pestaña) {
            document.getElementById('tab-recepcion').classList.toggle('hidden', pestaña !== 'recepcion');
            document.getElementById('tab-tecnicos').classList.toggle('hidden', pestaña !== 'tecnicos');
            document.getElementById('tab-finanzas').classList.toggle('hidden', pestaña !== 'finanzas');
            document.getElementById('tab-garantias').classList.toggle('hidden', pestaña !== 'garantias');

            const tabs = ['tab-btn-recepcion', 'tab-btn-tecnicos', 'tab-btn-finanzas', 'tab-btn-garantias'];
            tabs.forEach(t => {
                const el = document.getElementById(t);
                if(el) {
                    if(t === `tab-btn-${pestaña}`) {
                        el.className = "btn-compact bg-purple-600 text-white font-bold py-3 px-4 rounded-xl uppercase text-xs flex items-center justify-center gap-2";
                    } else {
                        el.className = "btn-compact bg-slate-900 text-slate-400 border border-slate-800 font-bold py-3 px-4 rounded-xl uppercase text-xs flex items-center justify-center gap-2";
                    }
                }
            });
        };

        // --- GUARDAR RECIBO CON ABONO ---
        window.svc_guardarComandaWorkspace = async function() {
            try {
                const operador = document.getElementById('form-operador').value;
                const cliente = document.getElementById('form-cliente').value.trim().toUpperCase();
                const cedula = document.getElementById('form-cedula').value.trim();
                const tlf = document.getElementById('form-tlf').value.trim();
                const tipoLinea = document.getElementById('form-tipo-linea').value;
                const modelo = document.getElementById('form-modelo').value.trim().toUpperCase();
                const falla = document.getElementById('form-falla').value.trim().toUpperCase();
                const claveManual = document.getElementById('form-clave-manual').value.trim().toUpperCase() || "N/A";
                const chkChip = document.getElementById('chk-chip').value;
                const chkMemoria = document.getElementById('chk-memoria').value;
                const chkForro = document.getElementById('chk-forro').value;
                const detallesManual = document.getElementById('form-detalles-manual').value.trim().toUpperCase() || "SIN DETALLES";
                const moneda = document.getElementById('form-moneda-base').value;
                const montoBase = parseFloat(document.getElementById('form-monto').value) || 0;
                const abonoBase = parseFloat(document.getElementById('form-abono').value) || 0;
                const tipoOp = document.getElementById('form-tipo-op').value;

                if(!cliente || !cedula || !modelo || montoBase <= 0) return alert("⚠️ Error: Complete los campos obligatorios.");

                const tCOP = parseFloat(document.getElementById('cfg-tasa-cop').value) || 3600;
                let usdEquiv = moneda === "USD" ? montoBase : montoBase / tCOP;
                let abonoUSDEquiv = moneda === "USD" ? abonoBase : abonoBase / tCOP;

                const nuevaComanda = {
                    id: 'ord-' + Date.now(),
                    nroOrden: String(svc_comandasGlobal.length + 1).padStart(3, '0'),
                    fecha: new Date().toLocaleDateString(),
                    hora: new Date().toLocaleTimeString([], { hour: '2-digit', minute: '2-digit' }),
                    cliente, cedula, tlf, tipoLinea, modelo, falla,
                    claveManual, fotoPatron: svc_fotoPatronBase64 || "",
                    chkChip, chkMemoria, chkForro, detallesManual,
                    monedaOrig: moneda, montoOrig: montoBase, abonoOrig: abonoBase,
                    montoUSD: usdEquiv, abonoUSD: abonoUSDEquiv,
                    tipoOp, operador, estatus: "RECIBIDO"
                };

                svc_comandasGlobal.push(nuevaComanda);

                // Limpiar campos
                document.getElementById('form-cliente').value = "";
                document.getElementById('form-cedula').value = "";
                document.getElementById('form-tlf').value = "";
                document.getElementById('form-modelo').value = "";
                document.getElementById('form-falla').value = "";
                document.getElementById('form-clave-manual').value = "";
                document.getElementById('form-detalles-manual').value = "";
                document.getElementById('form-monto').value = "";
                document.getElementById('form-abono').value = "0";
                document.getElementById('form-foto-patron').value = "";
                document.getElementById('wrapper-miniatura-patron').classList.add('hidden');
                svc_fotoPatronBase64 = "";

                await window.svc_sincronizarConFirebase();
                window.svc_renderizarEcosistema();
                window.svc_renderUltimoVisor(nuevaComanda);
            } catch(e) {}
        };

        window.svc_renderUltimoVisor = function(c) {
            const v = document.getElementById('wrapper-ultimo-visor');
            if(!v) return;
            
            let displayPendienteStr = "";
            let saldoRestante = c.montoOrig - c.abonoOrig;
            if(c.monedaOrig === "USD") {
                displayPendienteStr = `$${saldoRestante.toFixed(2)} USD`;
            } else {
                displayPendienteStr = `${Math.round(saldoRestante).toLocaleString()} COP`;
            }

            v.innerHTML = `
                <div class="space-y-3">
                    <div class="flex justify-between items-center border-b border-slate-900 pb-2">
                        <b class="text-white text-sm">Orden Nro #${c.nroOrden}</b>
                        <span class="text-[10px] bg-slate-900 px-2 py-0.5 rounded text-purple-400 font-mono font-bold">${c.fecha} - ${c.hora}</span>
                    </div>
                    <p class="text-slate-300">• Cliente: <strong class="text-white">${c.cliente} (C.I. ${c.cedula})</strong></p>
                    <p class="text-slate-300">• Equipo: <strong class="text-white">${c.modelo} — Falla: ${c.falla}</strong></p>
                    <p class="text-slate-300">• Resguardo: SIM: ${c.chkChip} | SD: ${c.chkMemoria} | Forro: ${c.chkForro}</p>
                    <p class="text-slate-300">• Clave: <span class="bg-slate-900 px-2 font-mono text-amber-400 border border-slate-800 rounded font-bold">${c.claveManual}</span></p>
                    
                    <div class="grid grid-cols-2 gap-2 bg-slate-900/60 p-2 rounded-xl border border-slate-850 text-center text-xs">
                        <div><span class="block text-[8px] text-slate-500 uppercase">Abonado</span><strong class="text-emerald-400 font-mono">${c.montoOrig === c.abonoOrig ? 'COMPLETO' : c.abonoOrig + ' ' + c.monedaOrig}</strong></div>
                        <div><span class="block text-[8px] text-red-400 uppercase font-black">Resta Cobrar</span><strong class="text-red-500 font-mono font-black">${displayPendienteStr}</strong></div>
                    </div>

                    ${c.fotoPatron ? `<div class="bg-slate-900 p-2 border border-slate-800 rounded-xl flex justify-center"><img src="${c.fotoPatron}" class="max-h-32 rounded-lg object-contain"></div>` : ''}
                    <p class="italic text-slate-400 text-xs">Obs: ${c.detallesManual}</p>
                    <div class="border-t border-slate-900 pt-2 flex justify-end">
                        <button onclick="window.svc_notificarTallerNelson(${svc_comandasGlobal.indexOf(c)})" class="bg-purple-600 hover:bg-purple-700 text-white text-[10px] font-black px-4 py-2.5 rounded-xl uppercase tracking-wider"><i class="fa-solid fa-paper-plane mr-1"></i> Despachar a Nelson</button>
                    </div>
                </div>`;
        };

        window.svc_notificarTallerNelson = function(idx) {
            const c = svc_comandasGlobal[idx];
            if(!c) return;
            let saldoRestante = c.montoOrig - c.abonoOrig;
            let displayPendiente = c.monedaOrig === "USD" ? `$${saldoRestante.toFixed(2)} USD` : `${Math.round(saldoRestante).toLocaleString()} COP`;
            
            let msg = `🛠 *NOTIFICACIÓN DE RECEPCIÓN — SERVICELL MASTER*\n\n`;
            msg += `Nelson, acabo de recibir en la oficina central el siguiente equipo. Por favor, verifica el mostrador físico cuando pase el cliente y déjalo ordenado en el taller bajo el número de *Orden #${c.nroOrden}*.\n\n`;
            msg += `📋 *Datos del Ingreso:*\n`;
            msg += `• *Cliente:* ${c.cliente} (C.I. ${c.cedula})\n`;
            msg += `• *Equipo:* ${c.modelo} | *Falla:* ${c.falla}\n`;
            msg += `• *SIM Card:* ${c.chkChip} | *SD:* ${c.chkMemoria} | *Forro:* ${c.chkForro}\n`;
            msg += `• *Clave de Acceso:* \`${c.claveManual}\`\n`;
            msg += `• *Abono:* ${c.abonoOrig} ${c.monedaOrig} | *Pendiente:* *${displayPendiente}*\n`;
            msg += `• *Detalles:* "${c.detallesManual}"\n\n`;
            msg += `👉 _El uso de este sistema es único y de su total responsabilidad._`;
            window.open(`https://api.whatsapp.com/send?text=${encodeURIComponent(msg)}`, '_blank');
        };

        // --- GESTIÓN DE TÉCNICOS ---
        window.svc_crearNuevoPerfilTecnicoMaster = async function() {
            const nombre = document.getElementById('adm-tec-nombre').value.trim();
            const user = document.getElementById('adm-tec-user').value.trim().toLowerCase();
            const pass = document.getElementById('adm-tec-pass').value.trim();
            const whatsapp = document.getElementById('adm-tec-whatsapp').value.trim();
            const comision = parseInt(document.getElementById('adm-tec-comision').value) || 50;

            if(!nombre || !user || !pass || !whatsapp) return alert("⚠️ Complete todos los campos.");

            const indexExist = svc_tecnicosPerfiles.findIndex(t => t.user === user);
            if(indexExist !== -1) {
                svc_tecnicosPerfiles[indexExist] = { nombre, user, pass, whatsapp, comision, estatus: "ACTIVO" };
            } else {
                svc_tecnicosPerfiles.push({ nombre, user, pass, whatsapp, comision, estatus: "ACTIVO" });
            }

            await setDoc(doc(db, "tcl_servicell_independent", "tecnicos_perfiles"), { perfiles: svc_tecnicosPerfiles });
            
            let urlUnica = `${window.location.href.split('?')[0]}`;
            let msg = `👑 *BIENVENIDO A SERVICEL MASTER — ALTA DE PERSONAL*\n\n`;
            msg += `Estimado colaborador, se hace entrega formal de su *enlace único de ingreso* al sistema de recepción y control técnico.\n\n`;
            msg += `⚠️ *REGLA DE OPERACIÓN OBLIGATORIA:* Todo trabajo técnico, desde el cambio de una pantalla hasta el más mínimo ajuste o revisión, debe ser ingresado en este enlace de manera ineludible.\n\n`;
            msg += `👤 *Credenciales de Entrada:*\n`;
            msg += `• *Enlace Único:* ${urlUnica}\n`;
            msg += `• *Usuario:* \`${user}\`\n`;
            msg += `• *Clave Temporal:* \`${pass}\`\n\n`;
            msg += `_Recuerde que el uso de esta infraestructura es personal y de su exclusiva responsabilidad._`;
            
            window.open(`https://api.whatsapp.com/send?phone=${whatsapp}&text=${encodeURIComponent(msg)}`, '_blank');

            document.getElementById('adm-tec-nombre').value = "";
            document.getElementById('adm-tec-user').value = "";
            document.getElementById('adm-tec-pass').value = "";
            document.getElementById('adm-tec-whatsapp').value = "";
            window.svc_renderizarEcosistema();
        };

        window.svc_eliminarPerfilTecnico = async function(idx) {
            if(!confirm("⚠️ ¿Desea revocar el perfil? Se mantendrá el expediente histórico legal intacto.")) return;
            svc_tecnicosPerfiles[idx].estatus = "REVOCADO";
            await setDoc(doc(db, "tcl_servicell_independent", "tecnicos_perfiles"), { perfiles: svc_tecnicosPerfiles });
            window.svc_renderizarEcosistema();
        };

        window.svc_reiniciarLinkAccesoTecnico = async function(idx) {
            let nuevaClave = "pass-" + Date.now();
            svc_tecnicosPerfiles[idx].pass = nuevaClave;
            await setDoc(doc(db, "tcl_servicell_independent", "tecnicos_perfiles"), { perfiles: svc_tecnicosPerfiles });
            window.svc_renderizarEcosistema();
            alert(`🔒 Enlace anterior revocado. La nueva contraseña para Nelson/Técnico es: ${nuevaClave}`);
        };

        window.svc_registrarValeColaborador = async function() {
            const tec = document.getElementById('form-vale-tecnico-dest').value;
            const monto = parseFloat(document.getElementById('form-vale-monto').value) || 0;
            if(!tec || monto <= 0) return alert("Datos del vale incorrectos.");

            svc_valesGlobal.push({ tec, monto, fecha: new Date().toLocaleDateString() });
            document.getElementById('form-vale-monto').value = "";
            await window.svc_sincronizarConFirebase();
            window.svc_renderizarEcosistema();
        };

        // --- RENDERIZADO GLOBAL ---
        window.svc_renderizarEcosistema = async function() {
            try {
                const tCOP = parseFloat(document.getElementById('cfg-tasa-cop').value) || 3600;
                const tBs = parseFloat(document.getElementById('cfg-tasa-bs').value) || 4;

                let totCOP = 0; let totUSD = 0; let totBs = 0;
                let totalNominasUSD = 0; let totalCajaTurnoUSD = 0;

                svc_comandasGlobal.forEach(f => {
                    if(f.estatus !== "ANULADA") {
                        // Para cálculo de cajas, sumamos solo lo que ingresó físicamente por el momento (Abono)
                        // A menos que ya esté ENTREGADA/FINALIZADA, en cuyo caso sumamos el valor total.
                        let ingresadoFisicoUSD = f.estatus === "FINALIZADO" ? f.montoUSD : f.abonoUSD;
                        let ingresadoFisicoMoneda = f.estatus === "FINALIZADO" ? f.montoOrig : f.abonoOrig;

                        totalCajaTurnoUSD += ingresadoFisicoUSD;

                        if(f.monedaOrig === "USD") {
                            totUSD += ingresadoFisicoMoneda;
                            totCOP += (ingresadoFisicoMoneda * tCOP);
                            totBs += (ingresadoFisicoMoneda * tCOP) / tBs;
                        } else if(f.monedaOrig === "COP") {
                            totCOP += ingresadoFisicoMoneda;
                            totUSD += ingresadoFisicoMoneda / tCOP;
                            totBs += ingresadoFisicoMoneda / tBs;
                        }

                        if(f.tipoOp === "SERVICIO") {
                            const tec = svc_tecnicosPerfiles.find(t => t.user === f.operador);
                            const coef = tec ? tec.comision / 100 : 0.50;
                            // La comisión final de nómina se calcula sobre el total de la reparación
                            totalNominasUSD += (f.montoUSD * coef);
                        }
                    }
                });

                let valesUSD = svc_valesGlobal.reduce((acc, v) => acc + v.monto, 0);
                let cajaNetaRealUSD = totalCajaTurnoUSD - valesUSD;

                // Actualizar cajas físicas en Finanzas
                const boxFin = document.getElementById('wrapper-fines-totales-moneda');
                if(boxFin) {
                    boxFin.innerHTML = `
                        <div class="bg-slate-900 border border-slate-800 p-4 rounded-2xl text-center shadow-md"><span class="text-[9px] font-black text-purple-400 block uppercase tracking-wider">🇨🇴 Caja Fiel COP</span><span class="text-base font-mono font-black text-white">${Math.round(totCOP).toLocaleString()} COP</span></div>
                        <div class="bg-slate-900 border border-slate-800 p-4 rounded-2xl text-center shadow-md"><span class="text-[9px] font-black text-amber-400 block uppercase tracking-wider">💵 Caja Fiel USD</span><span class="text-base font-mono font-black text-white">$${totUSD.toFixed(2)}</span></div>
                        <div class="bg-slate-900 border border-slate-800 p-4 rounded-2xl text-center shadow-md"><span class="text-[9px] font-black text-emerald-400 block uppercase tracking-wider">🇻🇪 PagoMóvil Bs</span><span class="text-base font-mono font-black text-white">${totBs.toFixed(2)} Bs</span></div>`;
                }

                if(document.getElementById('lbl-total-nominas')) document.getElementById('lbl-total-nominas').innerText = `$${totalNominasUSD.toFixed(2)}`;
                if(document.getElementById('lbl-total-caja-neta')) document.getElementById('lbl-total-caja-neta').innerText = `$${cajaNetaRealUSD.toFixed(2)}`;

                // Dropdown de Vales
                const dropdownVales = document.getElementById('form-vale-tecnico-dest');
                if(dropdownVales) {
                    dropdownVales.innerHTML = svc_tecnicosPerfiles.filter(t => t.estatus === 'ACTIVO').map(t => `<option value="${t.user}">${t.nombre.toUpperCase()}</option>`).join('');
                }

                const gridVales = document.getElementById('wrapper-vales-turno-grid');
                if(gridVales) {
                    gridVales.innerHTML = svc_valesGlobal.map(v => `<div class="bg-red-950/20 text-red-400 p-1.5 border border-red-900/10 rounded-lg flex justify-between mt-1"><span>Adelanto [${v.tec.toUpperCase()} - ${v.fecha}]</span><b>-$${v.monto.toFixed(2)}</b></div>`).join('');
                }

                // Selector de Responsable (Formulario de Recepción)
                const sOperador = document.getElementById('form-operador');
                if(sOperador) {
                    let opts = `<option value="MASTER">👑 MÁSTER (DUEÑO)</option>`;
                    svc_tecnicosPerfiles.filter(t => t.estatus === "ACTIVO").forEach(t => {
                        opts += `<option value="${t.user}">${t.nombre.toUpperCase()}</option>`;
                    });
                    sOperador.innerHTML = opts;
                    if(rolDeSesionActiva === "TECNICO") {
                        sOperador.value = usuarioSesionActivo;
                        sOperador.disabled = true;
                    }
                }

                // Render Fichas Técnicas
                const gridFichas = document.getElementById('wrapper-fichas-tecnicos-grid');
                if(gridFichas) {
                    gridFichas.innerHTML = "";
                    for (const [idx, t] of svc_tecnicosPerfiles.entries()) {
                        const docExp = await getDoc(doc(db, "tcl_servicell_independent", `expediente_${t.user}`));
                        let expHtml = `<p class="text-red-500 italic text-[10px]">Falta completar expediente legal obligatorio.</p>`;
                        if(docExp.exists()) {
                            const ed = docExp.data();
                            expHtml = `
                                <div class="bg-slate-950 p-2.5 rounded-xl border border-slate-900 space-y-1 text-[11px] text-slate-300 mt-1 font-mono">
                                    <p class="text-white">• C.I.: ${ed.cedula}</p>
                                    <p class="text-white">• WhatsApp: ${ed.whatsapp}</p>
                                    <p class="text-white">• Dirección: ${ed.direccion}</p>
                                </div>`;
                        }

                        gridFichas.innerHTML += `
                            <div class="p-4 bg-slate-950/40 border border-slate-800 rounded-2xl flex flex-col justify-between">
                                <div>
                                    <div class="flex justify-between items-start">
                                        <b class="text-white text-sm font-sans">${t.nombre.toUpperCase()}</b>
                                        <span class="text-[8px] font-black px-2 py-0.5 rounded uppercase ${t.estatus === 'ACTIVO' ? 'bg-emerald-600/10 text-emerald-400' : 'bg-red-600/10 text-red-400'}">${t.estatus}</span>
                                    </div>
                                    <span class="text-[10px] text-purple-400 font-mono block mt-1 font-bold">Comisión: ${t.comision}% | ID: ${t.user}</span>
                                    ${expHtml}
                                </div>
                                <div class="flex gap-2 justify-end mt-4 pt-2 border-t border-slate-900">
                                    <button onclick="window.svc_reiniciarLinkAccesoTecnico(${idx})" class="bg-slate-900 border border-slate-800 text-[10px] text-slate-300 font-bold px-3 py-1.5 rounded-xl uppercase">Revocar Link</button>
                                    ${t.estatus === 'ACTIVO' ? `<button onclick="window.svc_eliminarPerfilTecnico(${idx})" class="bg-red-600/10 border border-red-500/10 text-red-400 text-[10px] font-bold px-3 py-1.5 rounded-xl uppercase">Eliminar</button>` : ''}
                                </div>
                            </div>`;
                    }
                }

                window.svc_renderizarTablasDeComandas(svc_comandasGlobal);
            } catch(e) {}
        };

        window.svc_renderizarTablasDeComandas = function(lista) {
            const gridFines = document.getElementById('wrapper-comandas-finanzas-grid');
            const gridGars = document.getElementById('wrapper-comandas-garantias-grid');
            
            let stringHtml = "";
            if(lista.length === 0) {
                stringHtml = `<p class="text-center text-slate-500 italic py-16 text-sm">No hay comandas registradas en el sistema.</p>`;
                if(gridFines) gridFines.innerHTML = stringHtml;
                if(gridGars) gridGars.innerHTML = stringHtml;
                return;
            }

            lista.slice().reverse().forEach(c => {
                const indexReal = svc_comandasGlobal.indexOf(c);
                const esFin = c.estatus === "FINALIZADO";
                const esListo = c.estatus === "LISTO PARA RETIRO";
                const esAnulada = c.estatus === "ANULADA";
                
                let bgStyle = "bg-slate-950 border-slate-850 text-slate-300";
                let badgeStyle = "bg-purple-600 text-white";
                let badgeText = "RECIBIDO";

                if(esListo) {
                    bgStyle = "bg-amber-950/20 border-amber-500/20 text-amber-300";
                    badgeStyle = "bg-amber-600 text-slate-950 font-black";
                    badgeText = "LISTO PARA COBRAR";
                } else if(esFin) {
                    bgStyle = "bg-emerald-950/20 border-emerald-500/20 text-emerald-300";
                    badgeStyle = "bg-emerald-600 text-white";
                    badgeText = "ENTREGADO (CERRADO)";
                } else if(esAnulada) {
                    bgStyle = "bg-purple-950/20 border-purple-500/20 text-purple-400";
                    badgeStyle = "bg-purple-800 text-white";
                    badgeText = "ANULADA";
                }

                let saldoRestante = c.montoOrig - c.abonoOrig;
                let displayPendienteStr = c.monedaOrig === "USD" ? `$${saldoRestante.toFixed(2)} USD` : `${Math.round(saldoRestante).toLocaleString()} COP`;

                stringHtml += `
                    <div class="p-4 border rounded-2xl mb-2 flex justify-between items-center ${bgStyle}">
                        <div class="space-y-1">
                            <div class="flex items-center gap-2">
                                <b class="text-white text-sm font-sans">Orden Nro #${c.nroOrden} — ${c.cliente}</b>
                                <span class="text-[8px] px-2 py-0.5 rounded font-black ${badgeStyle}">${badgeText}</span>
                            </div>
                            <span class="text-xs block text-white mt-0.5">Equipo: <b>${c.modelo}</b> — Servicio: <b>${c.falla}</b></span>
                            <span class="text-[10px] block text-slate-400 font-mono">SIM: ${c.chkChip} | SD: ${c.chkMemoria} | Forro: ${c.chkForro} | Obs: ${c.detallesManual}</span>
                            <div class="flex gap-2 text-[10px] font-mono mt-0.5">
                                <span class="text-emerald-400">Abonó: ${c.abonoOrig} ${c.monedaOrig}</span>
                                ${saldoRestante > 0 && !esFin ? `<span class="text-red-400 font-black uppercase">Pendiente: ${displayPendienteStr}</span>` : '<span class="text-emerald-400 font-black uppercase">✔ PAGO TOTAL</span>'}
                            </div>
                        </div>
                        <div class="flex items-center gap-2 font-mono">
                            <div class="text-right">
                                <b class="text-white block text-sm">${c.montoOrig.toLocaleString()} ${c.monedaOrig}</b>
                                <span class="text-[9px] text-slate-500 block">Ref: $${c.montoUSD.toFixed(2)}</span>
                            </div>
                            ${rolDeSesionActiva === "MASTER" ? `<button onclick="window.svc_abrirAccionesComandaMaster(${indexReal})" class="bg-purple-600 hover:bg-purple-700 text-white w-8 h-8 rounded-xl flex items-center justify-center shadow"><i class="fa-solid fa-sliders text-sm"></i></button>` : ''}
                        </div>
                    </div>`;
            });

            if(gridFines) gridFines.innerHTML = stringHtml;
            if(gridGars) gridGars.innerHTML = stringHtml;
        };

        window.svc_filtrarComandasBuscador = function() {
            const mCriterio = document.getElementById('search-criterio').value.trim().toUpperCase();
            let filtradas = svc_comandasGlobal;
            if(mCriterio) {
                filtradas = svc_comandasGlobal.filter(c => c.cedula.includes(mCriterio) || c.cliente.includes(mCriterio) || c.nroOrden.includes(mCriterio) || c.modelo.includes(mCriterio));
            }
            window.svc_renderizarTablasDeComandas(filtradas);
        };

        // --- CONSOLA MÁSTER ACCIONES: RECIBIDO ➔ LISTO ➔ ENTREGADO ---
        window.svc_abrirAccionesComandaMaster = function(idx) {
            const c = svc_comandasGlobal[idx];
            if(!c) return;

            let promptText = `⚙️ AUDITORÍA MASTER — ORDEN #${c.nroOrden}\n\n`;
            promptText += `Escriba el número de la acción contable:\n`;
            promptText += `[1] Enviar Notificación de Recibido (WhatsApp)\n`;
            promptText += `[2] Enviar Notificación de "Listo para Retiro" (Cambiar Estatus)\n`;
            promptText += `[3] MARCAR COMO ENTREGADO (Cierre definitivo de saldo y dinero)\n`;
            promptText += `[4] Corregir Canal de Línea ( Nelson se equivocó: Alternar WhatsApp/Llamada )\n`;
            promptText += `[5] Anular Registro (Emitir Nota de Crédito)`;
            promptText += `\n\nPresione cancelar para salir.`;

            const s = prompt(promptText);
            const tCOP = parseFloat(document.getElementById('cfg-tasa-cop').value) || 3600;
            const tBs = parseFloat(document.getElementById('cfg-tasa-bs').value) || 4;

            if(s === "1") {
                let msg = `🛍️ *MOVISTAR CORDERO — SERVICEL MASTER RECEPCIÓN*\n\n`;
                msg += `Estimado cliente, le informamos que hemos recibido en Servicel Master, el servicio técnico autorizado de Tucocel de Movistar Cordero, un equipo en nuestro mostrador:\n\n`;
                msg += `📱 *Detalles del Dispositivo:*\n`;
                msg += `• Marca y Modelo: *${c.modelo}*\n`;
                msg += `• Soporte a Realizar: *${c.falla}*\n\n`;
                msg += `📊 *Ficha de Componentes en Resguardo:*\n`;
                msg += `• SIM Card / Chip: *${c.chkChip}*\n`;
                msg += `• Tarjeta SD: *${c.chkMemoria}*\n`;
                msg += `• Forro Protector: *${c.chkForro}*\n\n`;
                msg += `🔍 *Detalles Físicos Apreciados (Revisión Ocular):*\n_"${c.detallesManual}"_\n\n`;
                msg += `===============================\n`;
                msg += `🕒 _Al estar listo su equipo, se le enviará una segunda notificación automática para su retiro. Si detectamos otra falla aparte de la notificada, le llamaremos o escribiremos para su debida autorización._\n\n`;
                msg += `Gracias por poner su tecnología en nuestras manos corporativas. 🛡️`;

                let cleanTlf = c.tlf.replace(/\D/g, ''); if(!cleanTlf.startsWith('58')) cleanTlf = '58' + cleanTlf;
                window.open(`https://api.whatsapp.com/send?phone=${cleanTlf}&text=${encodeURIComponent(msg)}`, '_blank');

            } else if(s === "2") {
                let saldoRestante = c.montoOrig - c.abonoOrig;
                let displayPendienteStr = "";
                if(c.monedaOrig === "USD") {
                    displayPendienteStr = `$${saldoRestante.toFixed(2)} USD (o ${Math.round(saldoRestante * tCOP).toLocaleString()} Pesos COP)`;
                } else {
                    displayPendienteStr = `${Math.round(saldoRestante).toLocaleString()} COP (o ${(saldoRestante / tBs).toFixed(2)} Bs)`;
                }

                let msg = `📱 *¡SU EQUIPO ESTÁ LISTO PARA RETIRAR!* 🌟\n\n`;
                msg += `Estimado usuario, le informamos con agrado que el proceso de revisión y soporte técnico de su equipo ha sido *finalizado con éxito* en Servicel Master, el servicio técnico autorizado de Tucocel (Movistar Cordero) 🛡️.\n\n`;
                msg += `📝 *Detalle del Soporte Realizado:*\n`;
                msg += `• *Equipo:* ${c.modelo}\n`;
                msg += `• *Servicio ejecutado:* ${c.falla}\n\n`;
                msg += `💳 *Balance de Cuenta a Liquidar:*\n`;
                msg += `• *Total a pagar:* *${displayPendienteStr}*\n\n`;
                msg += `🕒 *Horario de Retiro:* Lunes a Sábado en nuestras instalaciones de mostrador.\n\n`;
                msg += `✨ _Queremos expresarle nuestro más sincero agradecimiento por confiar en nuestra labor y poner su tecnología en nuestras manos. Para nosotros es un absoluto placer ofrecerle el servicio corporativo de alta gama que usted se merece._\n\n`;
                msg += `¡Le esperamos para la entrega! 🤝`;

                let cleanTlf = c.tlf.replace(/\D/g, ''); if(!cleanTlf.startsWith('58')) cleanTlf = '58' + cleanTlf;
                window.open(`https://api.whatsapp.com/send?phone=${cleanTlf}&text=${encodeURIComponent(msg)}`, '_blank');

                svc_comandasGlobal[idx].estatus = "LISTO PARA RETIRO";
                window.svc_sincronizarConFirebase();
                window.svc_renderizarEcosistema();

            } else if(s === "3") {
                if(!confirm("🤝 ¿Desea registrar el saldo restante y despachar el equipo como ENTREGADO y pagado completo? El saldo se sumará a tus cajas.")) return;
                
                svc_comandasGlobal[idx].estatus = "FINALIZADO";
                window.svc_sincronizarConFirebase();
                window.svc_renderizarEcosistema();
                alert("✅ Equipo marcado como ENTREGADO. Balance contable actualizado.");

            } else if(s === "4") {
                let old = svc_comandasGlobal[idx].tipoLinea;
                svc_comandasGlobal[idx].tipoLinea = old === "WHATSAPP" ? "LLAMADA" : "WHATSAPP";
                window.svc_sincronizarConFirebase();
                window.svc_renderizarEcosistema();
                alert("Canal de línea rectificado en servidor.");
            } else if(s === "5") {
                if(!confirm("¿Desea anular la comanda y emitir nota de crédito?")) return;
                svc_comandasGlobal[idx].estatus = "ANULADA";
                window.svc_sincronizarConFirebase();
                window.svc_renderizarEcosistema();
            }
        };

        window.svc_ejecutarCierreSemanalTotalHistorico = async function() {
            if(!confirm("🔒 ¿Cerrar semana contable? Se guardará en el histórico inalterable de la nube.")) return;
            svc_cierresGlobal.push({
                fechaCierre: new Date().toLocaleDateString(),
                comandas: [...svc_comandasGlobal],
                vales: [...svc_valesGlobal]
            });
            svc_comandasGlobal = [];
            svc_valesGlobal = [];
            await window.svc_sincronizarConFirebase();
            window.svc_renderizarEcosistema();
            alert("⚙️ Turno cerrado e indexado correctamente.");
        };

        window.svc_sincronizarConFirebase = async function() {
            try {
                await setDoc(doc(db, "tcl_servicell_independent", "comandas_data"), {
                    comandas: svc_comandasGlobal,
                    vales: svc_valesGlobal,
                    historico: svc_cierresGlobal
                });
            } catch(e) {}
        };
    </script>
</body>
</html>
